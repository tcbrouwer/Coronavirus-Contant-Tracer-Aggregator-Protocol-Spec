# DP3T HTTP Implementation Profile

## Overview for app developers

To check for infection: first load the list of data dumps from /exposed.

	for each (dump-you-havent-processed-or-which-has-a-new-hash)

		load data from `uri_filter` into your cocofilter
		run your local interactions through the cocofilter.

		if ( interaction in cocofilter )
			download the big list of ids from uri_data and check them
		else
			stop you're not exposed

# Endpoints

## /exposed

	GET /{version}/exposed

Response:

	application/json

	{
		[{
			time_stamp_from: 'isodatetime',
			time_stamp_to: 'iso',
			hash: 'hash_which_identifies_this_for_changes'
			uri_filter: '/whatever/the/uri/is/for/the/coocoofilter'
			uri_data: '/whatever/the/uri/is/for/the/big/binary'
		}, ...]

	}

### Response description

	Returns an json array containing a list of data batches in reverse-chronological order - so the latest update comes first. The timespan of the file is included along with a relative url to the coco filter binary and to the data file binary. The hash identifies the uri_data and thus changes if the data changes (so mistakes can be fixed).

### Request fields

See request-fields.md

### Response fields

See response-fields.md

## /exposed/filter

	GET /{version}/exposed/{batch-id}/filter

Response:

	application/octet-stream

	<example CocoFilterFormat>

Response description:

	Some text


## /exposed/data

	GET /{version}/exposed/{batch-id}/data

	application/octet-stream

	<example ExposedDeviceIdentifiersFormat>


# Messages

## CoCoFilterFormat

Define it.

## ExposedDeviceIdentifiersFormat

Define it.


