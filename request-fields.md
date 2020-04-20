Request fields
--------------

### Standard request fields

```
+-------------+-------------+-------------+-------------+-------------+
| Name        | Description | Example     | Status      | Standard    |
+=============+=============+=============+=============+=============+
| A-IM        | Acceptable  | `A-IM: feed | Permanent   | ```{=mediaw |
|             | instance-ma | `           |             | iki}        |
|             | nipulations |             |             | {{IETF RFC| |
|             | for the     |             |             | 3229}}      |
|             | request.[^1 |             |             | ```         |
|             | 0]          |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Accept      | [Media      | `Accept: te | Permanent   | ```{=mediaw |
|             | type(s)](Me | xt/html`    |             | iki}        |
|             | dia_type "w |             |             | {{IETF RFC| |
|             | ikilink")   |             |             | 2616|7231}} |
|             | that is/are |             |             | ```         |
|             | acceptable  |             |             |             |
|             | for the     |             |             |             |
|             | response.   |             |             |             |
|             | See         |             |             |             |
|             | [Content    |             |             |             |
|             | negotiation |             |             |             |
|             | ](Content_n |             |             |             |
|             | egotiation  |             |             |             |
|             | "wikilink") |             |             |             |
|             | .           |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Accept-Char | Character   | `Accept-Cha | Permanent   | ```{=mediaw |
| set         | sets that   | rset: utf-8 |             | iki}        |
|             | are         | `           |             | {{IETF RFC| |
|             | acceptable. |             |             | 2616|}}     |
|             |             |             |             | ```         |
+-------------+-------------+-------------+-------------+-------------+
| Accept-Date | Acceptable  | `Accept-Dat | Provisional | ```{=mediaw |
| time        | version in  | etime: Thu, |             | iki}        |
|             | time.       |  31 May 200 |             | {{IETF RFC| |
|             |             | 7 20:35:00  |             | 7089|}}     |
|             |             | GMT`        |             | ```         |
+-------------+-------------+-------------+-------------+-------------+
| Accept-Enco | List of     | `Accept-Enc | Permanent   | ```{=mediaw |
| ding        | acceptable  | oding: gzip |             | iki}        |
|             | encodings.  | , deflate`  |             | {{IETF RFC| |
|             | See [HTTP   |             |             | 2616|7231}} |
|             | compression |             |             | ```         |
|             | ](HTTP_comp |             |             |             |
|             | ression "wi |             |             |             |
|             | kilink").   |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Accept-Lang | List of     | `Accept-Lan | Permanent   | ```{=mediaw |
| uage        | acceptable  | guage: en-U |             | iki}        |
|             | human       | S`          |             | {{IETF RFC| |
|             | languages   |             |             | 2616|7231}} |
|             | for         |             |             | ```         |
|             | response.   |             |             |             |
|             | See         |             |             |             |
|             | [Content    |             |             |             |
|             | negotiation |             |             |             |
|             | ](Content_n |             |             |             |
|             | egotiation  |             |             |             |
|             | "wikilink") |             |             |             |
|             | .           |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| ```{=mediaw | Initiates a | `Access-Con | ```{=mediaw |             |
| iki}        | request for | trol-Reques | iki}        |             |
| {{nowrap|Ac | [cross-orig | t-Method: G | {{nowrap|Pe |             |
| cess-Contro | in          | ET`         | rmanent: st |             |
| l-Request-M | resource    |             | andard}}    |             |
| ethod,<br / | sharing](cr |             | ```         |             |
| >Access-Con | oss-origin_ |             |             |             |
| trol-Reques | resource_sh |             |             |             |
| t-Headers}} | aring "wiki |             |             |             |
| ```         | link")      |             |             |             |
| [^11]       | with        |             |             |             |
|             | [Origin](#o |             |             |             |
|             | rigin-reque |             |             |             |
|             | st-header " |             |             |             |
|             | wikilink")  |             |             |             |
|             | (below).    |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Authorizati | Authenticat | `Authorizat | Permanent   |             |
| on          | ion         | ion: Basic  |             |             |
|             | credentials | QWxhZGRpbjp |             |             |
|             | for [HTTP   | vcGVuIHNlc2 |             |             |
|             | authenticat | FtZQ==`     |             |             |
|             | ion](Basic_ |             |             |             |
|             | access_auth |             |             |             |
|             | entication  |             |             |             |
|             | "wikilink") |             |             |             |
|             | .           |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| [Cache-Cont | Used to     | `Cache-Cont | Permanent   |             |
| rol](Cache- | specify     | rol: no-cac |             |             |
| Control "wi | directives  | he`         |             |             |
| kilink")    | that *must* |             |             |             |
|             | be obeyed   |             |             |             |
|             | by all      |             |             |             |
|             | caching     |             |             |             |
|             | mechanisms  |             |             |             |
|             | along the   |             |             |             |
|             | request-res |             |             |             |
|             | ponse       |             |             |             |
|             | chain.      |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Connection  | Control     | url=<http:/ | title=Hyper | publisher=[ |
|             | options for | /tools.ietf | text        | IETF](IETF  |
|             | the current | .org/html/r | Transfer    | "wikilink") |
|             | connection  | fc7230#sect | Protocol    |             |
|             | and list of | ion-6.1>    | (HTTP/1.1): |             |
|             | hop-by-hop  |             | Message     |             |
|             | request     |             | Syntax and  |             |
|             | fields.<ref |             | Routing     |             |
|             |  name="rfc7 |             |             |             |
|             | 230_connect |             |             |             |
|             | ion">{{cite |             |             |             |
|             | web         |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Content-Enc | The type of | `Content-En | Permanent   |             |
| oding       | encoding    | coding: gzi |             |             |
|             | used on the | p`          |             |             |
|             | data. See   |             |             |             |
|             | [HTTP       |             |             |             |
|             | compression |             |             |             |
|             | ](HTTP_comp |             |             |             |
|             | ression "wi |             |             |             |
|             | kilink").   |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Content-Len | The length  | `Content-Le | Permanent   |             |
| gth         | of the      | ngth: 348`  |             |             |
|             | request     |             |             |             |
|             | body in     |             |             |             |
|             | [octets](Oc |             |             |             |
|             | tet_(comput |             |             |             |
|             | ing) "wikil |             |             |             |
|             | ink")       |             |             |             |
|             | (8-bit      |             |             |             |
|             | bytes).     |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Content-MD5 | A           | `Content-MD | Obsolete[^1 |             |
|             | [Base64](Ba | 5: Q2hlY2sg | 2]          |             |
|             | se64 "wikil | SW50ZWdyaXR |             |             |
|             | ink")-encod | 5IQ==`      |             |             |
|             | ed          |             |             |             |
|             | binary      |             |             |             |
|             | [MD5](MD5 " |             |             |             |
|             | wikilink")  |             |             |             |
|             | sum of the  |             |             |             |
|             | content of  |             |             |             |
|             | the request |             |             |             |
|             | body.       |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Content-Typ | The [Media  | `Content-Ty | Permanent   |             |
| e           | type](Media | pe: applica |             |             |
|             | _type "wiki | tion/x-www- |             |             |
|             | link")      | form-urlenc |             |             |
|             | of the body | oded`       |             |             |
|             | of the      |             |             |             |
|             | request     |             |             |             |
|             | (used with  |             |             |             |
|             | POST and    |             |             |             |
|             | PUT         |             |             |             |
|             | requests).  |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Cookie      | An [HTTP    | `Cookie: $V | Permanent:  |             |
|             | cookie](HTT | ersion=1; S | standard    |             |
|             | P_cookie "w | kin=new;`   |             |             |
|             | ikilink")   |             |             |             |
|             | previously  |             |             |             |
|             | sent by the |             |             |             |
|             | server with |             |             |             |
|             | [`Set-Cooki |             |             |             |
|             | e`](#innerl |             |             |             |
|             | ink_set-coo |             |             |             |
|             | kie "wikili |             |             |             |
|             | nk")        |             |             |             |
|             | (below).    |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Date        | The date    | `Date: Tue, | Permanent   |             |
|             | and time at |  15 Nov 199 |             |             |
|             | which the   | 4 08:12:31  |             |             |
|             | message was | GMT`        |             |             |
|             | originated  |             |             |             |
|             | (in         |             |             |             |
|             | \"HTTP-date |             |             |             |
|             | \"          |             |             |             |
|             | format as   |             |             |             |
|             | defined by  |             |             |             |
|             | [RFC 7231   |             |             |             |
|             | Date/Time   |             |             |             |
|             | Formats](ht |             |             |             |
|             | tp://tools. |             |             |             |
|             | ietf.org/ht |             |             |             |
|             | ml/rfc7231# |             |             |             |
|             | section-7.1 |             |             |             |
|             | .1.1)).     |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Expect      | Indicates   | `Expect: 10 | Permanent   |             |
|             | that        | 0-continue` |             |             |
|             | particular  |             |             |             |
|             | server      |             |             |             |
|             | behaviors   |             |             |             |
|             | are         |             |             |             |
|             | required by |             |             |             |
|             | the client. |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Forwarded   | Disclose    | url=<http:/ | title=Forwa | publisher=[ |
|             | original    | /tools.ietf | rded        | IETF](IETF  |
|             | information | .org/html/r | HTTP        | "wikilink") |
|             | of a client | fc7239#sect | Extension:  |             |
|             | connecting  | ion-1>      | Introductio |             |
|             | to a web    |             | n           |             |
|             | server      |             |             |             |
|             | through an  |             |             |             |
|             | HTTP        |             |             |             |
|             | proxy.<ref> |             |             |             |
|             | {{cite      |             |             |             |
|             | web         |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| From        | The email   | `From: user | Permanent   |             |
|             | address of  | @example.co |             |             |
|             | the user    | m`          |             |             |
|             | making the  |             |             |             |
|             | request.    |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Host        | The domain  | url=<http:/ | title=Hyper | publisher=[ |
|             | name of the | /tools.ietf | text        | IETF](IETF  |
|             | server (for | .org/html/r | Transfer    | "wikilink") |
|             | [virtual    | fc7230#sect | Protocol    |             |
|             | hosting](vi | ion-5.4>    | (HTTP/1.1): |             |
|             | rtual_hosti |             | Message     |             |
|             | ng "wikilin |             | Syntax and  |             |
|             | k")),       |             | Routing     |             |
|             | and the     |             |             |             |
|             | [TCP        |             |             |             |
|             | port](List_ |             |             |             |
|             | of_TCP_and_ |             |             |             |
|             | UDP_port_nu |             |             |             |
|             | mbers "wiki |             |             |             |
|             | link")      |             |             |             |
|             | number on   |             |             |             |
|             | which the   |             |             |             |
|             | server is   |             |             |             |
|             | listening.  |             |             |             |
|             | The         |             |             |             |
|             | [port](Port |             |             |             |
|             | _(computer_ |             |             |             |
|             | networking) |             |             |             |
|             |  "wikilink" |             |             |             |
|             | )           |             |             |             |
|             | number may  |             |             |             |
|             | be omitted  |             |             |             |
|             | if the port |             |             |             |
|             | is the      |             |             |             |
|             | standard    |             |             |             |
|             | port for    |             |             |             |
|             | the service |             |             |             |
|             | requested.  |             |             |             |
|             | Mandatory   |             |             |             |
|             | since       |             |             |             |
|             | HTTP/1.1.<r |             |             |             |
|             | ef>{{cite   |             |             |             |
|             | web         |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| HTTP2-Setti | A request   | `HTTP2-Sett | Permanent:  |             |
| ngs         | that        | ings: token | standard    |             |
|             | upgrades    | 64`         |             |             |
|             | from        |             |             |             |
|             | HTTP/1.1 to |             |             |             |
|             | HTTP/2 MUST |             |             |             |
|             | include     |             |             |             |
|             | exactly one |             |             |             |
|             | `HTTP2-Sett |             |             |             |
|             | ing`        |             |             |             |
|             | header      |             |             |             |
|             | field. The  |             |             |             |
|             | `HTTP2-Sett |             |             |             |
|             | ings`       |             |             |             |
|             | header      |             |             |             |
|             | field is a  |             |             |             |
|             | connection- |             |             |             |
|             | specific    |             |             |             |
|             | header      |             |             |             |
|             | field that  |             |             |             |
|             | includes    |             |             |             |
|             | parameters  |             |             |             |
|             | that govern |             |             |             |
|             | the HTTP/2  |             |             |             |
|             | connection, |             |             |             |
|             | provided in |             |             |             |
|             | anticipatio |             |             |             |
|             | n           |             |             |             |
|             | of the      |             |             |             |
|             | server      |             |             |             |
|             | accepting   |             |             |             |
|             | the request |             |             |             |
|             | to          |             |             |             |
|             | upgrade.[^1 |             |             |             |
|             | 3][^14]     |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| If-Match    | Only        | `If-Match:  | Permanent   |             |
|             | perform the | "737060cd8c |             |             |
|             | action if   | 284d8af7ad3 |             |             |
|             | the client  | 082f209582d |             |             |
|             | supplied    | "`          |             |             |
|             | entity      |             |             |             |
|             | matches the |             |             |             |
|             | same entity |             |             |             |
|             | on the      |             |             |             |
|             | server.     |             |             |             |
|             | This is     |             |             |             |
|             | mainly for  |             |             |             |
|             | methods     |             |             |             |
|             | like PUT to |             |             |             |
|             | only update |             |             |             |
|             | a resource  |             |             |             |
|             | if it has   |             |             |             |
|             | not been    |             |             |             |
|             | modified    |             |             |             |
|             | since the   |             |             |             |
|             | user last   |             |             |             |
|             | updated it. |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| If-Modified | Allows a    | `If-Modifie | Permanent   |             |
| -Since      | *304 Not    | d-Since: Sa |             |             |
|             | Modified*   | t, 29 Oct 1 |             |             |
|             | to be       | 994 19:43:3 |             |             |
|             | returned if | 1 GMT`      |             |             |
|             | content is  |             |             |             |
|             | unchanged.  |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| If-None-Mat | Allows a    | `If-None-Ma | Permanent   |             |
| ch          | *304 Not    | tch: "73706 |             |             |
|             | Modified*   | 0cd8c284d8a |             |             |
|             | to be       | f7ad3082f20 |             |             |
|             | returned if | 9582d"`     |             |             |
|             | content is  |             |             |             |
|             | unchanged,  |             |             |             |
|             | see [HTTP   |             |             |             |
|             | ETag](HTTP_ |             |             |             |
|             | ETag "wikil |             |             |             |
|             | ink").      |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| If-Range    | If the      | `If-Range:  | Permanent   |             |
|             | entity is   | "737060cd8c |             |             |
|             | unchanged,  | 284d8af7ad3 |             |             |
|             | send me the | 082f209582d |             |             |
|             | part(s)     | "`          |             |             |
|             | that I am   |             |             |             |
|             | missing;    |             |             |             |
|             | otherwise,  |             |             |             |
|             | send me the |             |             |             |
|             | entire new  |             |             |             |
|             | entity.     |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| If-Unmodifi | Only send   | `If-Unmodif | Permanent   |             |
| ed-Since    | the         | ied-Since:  |             |             |
|             | response if | Sat, 29 Oct |             |             |
|             | the entity  |  1994 19:43 |             |             |
|             | has not     | :31 GMT`    |             |             |
|             | been        |             |             |             |
|             | modified    |             |             |             |
|             | since a     |             |             |             |
|             | specific    |             |             |             |
|             | time.       |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Max-Forward | Limit the   | `Max-Forwar | Permanent   |             |
| s           | number of   | ds: 10`     |             |             |
|             | times the   |             |             |             |
|             | message can |             |             |             |
|             | be          |             |             |             |
|             | forwarded   |             |             |             |
|             | through     |             |             |             |
|             | proxies or  |             |             |             |
|             | gateways.   |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Origin[^15] | Initiates a | `Origin: ht | Permanent:  |             |
|             | request for | tp://www.ex | standard    |             |
|             | [cross-orig | ample-socia |             |             |
|             | in          | l-network.c |             |             |
|             | resource    | om`         |             |             |
|             | sharing](cr |             |             |             |
|             | oss-origin_ |             |             |             |
|             | resource_sh |             |             |             |
|             | aring "wiki |             |             |             |
|             | link")      |             |             |             |
|             | (asks       |             |             |             |
|             | server for  |             |             |             |
|             | [Access-Con |             |             |             |
|             | trol-\*](#a |             |             |             |
|             | ccess-contr |             |             |             |
|             | ol-response |             |             |             |
|             | -headers "w |             |             |             |
|             | ikilink")   |             |             |             |
|             | response    |             |             |             |
|             | fields).    |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Pragma      | Implementat | [`Pragma:`` | Permanent   |             |
|             | ion-specifi |  ``no-cache |             |             |
|             | c           | `](#Avoidin |             |             |
|             | fields that | g_caching " |             |             |
|             | may have    | wikilink")  |             |             |
|             | various     |             |             |             |
|             | effects     |             |             |             |
|             | anywhere    |             |             |             |
|             | along the   |             |             |             |
|             | request-res |             |             |             |
|             | ponse       |             |             |             |
|             | chain.      |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Proxy-Autho | Authorizati | `Proxy-Auth | Permanent   |             |
| rization    | on          | orization:  |             |             |
|             | credentials | Basic QWxhZ |             |             |
|             | for         | GRpbjpvcGVu |             |             |
|             | connecting  | IHNlc2FtZQ= |             |             |
|             | to a proxy. | =`          |             |             |
+-------------+-------------+-------------+-------------+-------------+
| ```{=mediaw | Request     | `Range: byt | Permanent   |             |
| iki}        | only part   | es=500-999` |             |             |
| {{anchor|Ra | of an       |             |             |             |
| nge}}       | entity.     |             |             |             |
| ```         | Bytes are   |             |             |             |
| Range       | numbered    |             |             |             |
|             | from 0. See |             |             |             |
|             | [Byte       |             |             |             |
|             | serving](By |             |             |             |
|             | te_serving  |             |             |             |
|             | "wikilink") |             |             |             |
|             | .           |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| [Referer](H | This is the | `Referer: h | Permanent   |             |
| TTP_referer | address of  | ttp://en.wi |             |             |
|  "wikilink" | the         | kipedia.org |             |             |
| )`{{sic}}`{ | previous    | /wiki/Main_ |             |             |
| =mediawiki} | web page    | Page`       |             |             |
|             | from which  |             |             |             |
|             | a link to   |             |             |             |
|             | the         |             |             |             |
|             | currently   |             |             |             |
|             | requested   |             |             |             |
|             | page was    |             |             |             |
|             | followed.   |             |             |             |
|             | (The word   |             |             |             |
|             | \"referrer\ |             |             |             |
|             | "           |             |             |             |
|             | has been    |             |             |             |
|             | misspelled  |             |             |             |
|             | in the RFC  |             |             |             |
|             | as well as  |             |             |             |
|             | in most     |             |             |             |
|             | implementat |             |             |             |
|             | ions        |             |             |             |
|             | to the      |             |             |             |
|             | point that  |             |             |             |
|             | it has      |             |             |             |
|             | become      |             |             |             |
|             | standard    |             |             |             |
|             | usage and   |             |             |             |
|             | is          |             |             |             |
|             | considered  |             |             |             |
|             | correct     |             |             |             |
|             | terminology |             |             |             |
|             | )           |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| TE          | The         | `TE: traile | Permanent   |             |
|             | transfer    | rs, `[`defl |             |             |
|             | encodings   | ate`](defla |             |             |
|             | the user    | te "wikilin |             |             |
|             | agent is    | k")         |             |             |
|             | willing to  |             |             |             |
|             | accept: the |             |             |             |
|             | same values |             |             |             |
|             | as for the  |             |             |             |
|             | response    |             |             |             |
|             | header      |             |             |             |
|             | field       |             |             |             |
|             | Transfer-En |             |             |             |
|             | coding      |             |             |             |
|             | can be      |             |             |             |
|             | used, plus  |             |             |             |
|             | the         |             |             |             |
|             | \"trailers\ |             |             |             |
|             | "           |             |             |             |
|             | value       |             |             |             |
|             | (related to |             |             |             |
|             | the         |             |             |             |
|             | \"[chunked] |             |             |             |
|             | (chunked_tr |             |             |             |
|             | ansfer_enco |             |             |             |
|             | ding "wikil |             |             |             |
|             | ink")\"     |             |             |             |
|             | transfer    |             |             |             |
|             | method) to  |             |             |             |
|             | notify the  |             |             |             |
|             | server it   |             |             |             |
|             | expects to  |             |             |             |
|             | receive     |             |             |             |
|             | additional  |             |             |             |
|             | fields in   |             |             |             |
|             | the trailer |             |             |             |
|             | after the   |             |             |             |
|             | last,       |             |             |             |
|             | zero-sized, |             |             |             |
|             | chunk. Only |             |             |             |
|             | `trailers`  |             |             |             |
|             | is          |             |             |             |
|             | supported   |             |             |             |
|             | in          |             |             |             |
|             | HTTP/2.[^16 |             |             |             |
|             | ]           |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Trailer     | The Trailer | `Trailer: M | Permanent   |             |
|             | general     | ax-Forwards |             |             |
|             | field value | `           |             |             |
|             | indicates   |             |             |             |
|             | that the    |             |             |             |
|             | given set   |             |             |             |
|             | of header   |             |             |             |
|             | fields is   |             |             |             |
|             | present in  |             |             |             |
|             | the trailer |             |             |             |
|             | of a        |             |             |             |
|             | message     |             |             |             |
|             | encoded     |             |             |             |
|             | with        |             |             |             |
|             | [chunked    |             |             |             |
|             | transfer    |             |             |             |
|             | coding](chu |             |             |             |
|             | nked_transf |             |             |             |
|             | er_coding " |             |             |             |
|             | wikilink"). |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Transfer-En | The form of | `Transfer-E | Permanent   |             |
| coding      | encoding    | ncoding: ch |             |             |
|             | used to     | unked`      |             |             |
|             | safely      |             |             |             |
|             | transfer    |             |             |             |
|             | the entity  |             |             |             |
|             | to the      |             |             |             |
|             | user.       |             |             |             |
|             | [Currently  |             |             |             |
|             | defined     |             |             |             |
|             | methods](ht |             |             |             |
|             | tp://www.ia |             |             |             |
|             | na.org/assi |             |             |             |
|             | gnments/htt |             |             |             |
|             | p-parameter |             |             |             |
|             | s)          |             |             |             |
|             | are:        |             |             |             |
|             | [chunked](c |             |             |             |
|             | hunked_tran |             |             |             |
|             | sfer_encodi |             |             |             |
|             | ng "wikilin |             |             |             |
|             | k"),        |             |             |             |
|             | compress,   |             |             |             |
|             | deflate,    |             |             |             |
|             | gzip,       |             |             |             |
|             | identity.   |             |             |             |
|             | Must not be |             |             |             |
|             | used with   |             |             |             |
|             | HTTP/2.[^17 |             |             |             |
|             | ]           |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| User-Agent  | The [user   | `User-Agent | Permanent   |             |
|             | agent       | : Mozilla/5 |             |             |
|             | string](use | .0 (X11; Li |             |             |
|             | r_agent_str | nux x86_64; |             |             |
|             | ing "wikili |  rv:12.0) G |             |             |
|             | nk")        | ecko/201001 |             |             |
|             | of the user | 01 Firefox/ |             |             |
|             | agent.      | 12.0`       |             |             |
+-------------+-------------+-------------+-------------+-------------+
| [Upgrade](U | Ask the     | `Upgrade: h | Permanent   |             |
| pgrade_head | server to   | 2c, HTTPS/1 |             |             |
| er "wikilin | upgrade to  | .3, IRC/6.9 |             |             |
| k")         | another     | , RTA/x11,  |             |             |
|             | protocol.   | websocket`  |             |             |
|             | Must not be |             |             |             |
|             | used in     |             |             |             |
|             | HTTP/2.[^18 |             |             |             |
|             | ]           |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Via         | Informs the | `Via: 1.0 f | Permanent   |             |
|             | server of   | red, 1.1 ex |             |             |
|             | proxies     | ample.com ( |             |             |
|             | through     | Apache/1.1) |             |             |
|             | which the   | `           |             |             |
|             | request was |             |             |             |
|             | sent.       |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Warning     | A general   | `Warning: 1 | Permanent   |             |
|             | warning     | 99 Miscella |             |             |
|             | about       | neous warni |             |             |
|             | possible    | ng`         |             |             |
|             | problems    |             |             |             |
|             | with the    |             |             |             |
|             | entity      |             |             |             |
|             | body.       |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
```
### Common non-standard request fields

```
+-----------------------+-----------------------+-----------------------+
| Field name            | Description           | Example               |
+=======================+=======================+=======================+
| ```{=mediawiki}       | Tells a server which  | `Upgrade-Insecure-Req |
| {{nowrap|Upgrade-Inse | (presumably in the    | uests: 1`             |
| cure-Requests}}       | middle of a HTTP -\>  |                       |
| ```                   | HTTPS migration)      |                       |
| [^44]                 | hosts mixed content   |                       |
|                       | that the client would |                       |
|                       | prefer redirection to |                       |
|                       | HTTPS and can handle  |                       |
|                       | `Content-Security-Pol |                       |
|                       | icy: upgrade-insecure |                       |
|                       | -requests`            |                       |
|                       | Must not be used with |                       |
|                       | HTTP/2[^45]           |                       |
+-----------------------+-----------------------+-----------------------+
| X-Requested-With      | Mainly used to        | `X-Requested-With: XM |
|                       | identify              | LHttpRequest`         |
|                       | [Ajax](Ajax_(programm |                       |
|                       | ing) "wikilink")      |                       |
|                       | requests. Most        |                       |
|                       | [JavaScript           |                       |
|                       | frameworks](JavaScrip |                       |
|                       | t_framework "wikilink |                       |
|                       | ")                    |                       |
|                       | send this field with  |                       |
|                       | value of              |                       |
|                       | `XMLHttpRequest`      |                       |
+-----------------------+-----------------------+-----------------------+
| [DNT](Do_Not_Track "w | Requests a web        | `DNT: 1` (Do Not      |
| ikilink")[^46]        | application to        | Track Enabled)        |
|                       | disable their         | `DNT: 0` (Do Not      |
|                       | tracking of a user.   | Track Disabled)       |
|                       | This is Mozilla\'s    |                       |
|                       | version of the        |                       |
|                       | X-Do-Not-Track header |                       |
|                       | field (since [Firefox |                       |
|                       | 4.0](Mozilla_Firefox_ |                       |
|                       | 4 "wikilink")         |                       |
|                       | Beta 11).             |                       |
|                       | [Safari](Safari_(web_ |                       |
|                       | browser) "wikilink")  |                       |
|                       | and                   |                       |
|                       | [IE9](Internet_Explor |                       |
|                       | er_9 "wikilink")      |                       |
|                       | also have support for |                       |
|                       | this field.[^47] On   |                       |
|                       | March 7, 2011, a      |                       |
|                       | draft proposal was    |                       |
|                       | submitted to          |                       |
|                       | IETF.[^48] The        |                       |
|                       | [W3C](World_Wide_Web_ |                       |
|                       | Consortium "wikilink" |                       |
|                       | )                     |                       |
|                       | Tracking Protection   |                       |
|                       | Working Group is      |                       |
|                       | producing a           |                       |
|                       | specification.[^49]   |                       |
+-----------------------+-----------------------+-----------------------+
| [X-Forwarded-For](X-F | A [*de facto*         | `X-Forwarded-For: cli |
| orwarded-For "wikilin | standard](de_facto_st | ent1, proxy1, proxy2` |
| k")[^50]              | andard "wikilink")    | `X-Forwarded-For: 129 |
|                       | for identifying the   | .78.138.66, 129.78.64 |
|                       | originating IP        | .103`                 |
|                       | address of a client   |                       |
|                       | connecting to a web   |                       |
|                       | server through an     |                       |
|                       | HTTP proxy or load    |                       |
|                       | balancer. Superseded  |                       |
|                       | by *Forwarded*        |                       |
|                       | header.               |                       |
+-----------------------+-----------------------+-----------------------+
| X-Forwarded-Host[^51] | A [*de facto*         | `X-Forwarded-Host: en |
|                       | standard](de_facto_st | .wikipedia.org:8080`  |
|                       | andard "wikilink")    | `X-Forwarded-Host: en |
|                       | for identifying the   | .wikipedia.org`       |
|                       | original host         |                       |
|                       | requested by the      |                       |
|                       | client in the `Host`  |                       |
|                       | HTTP request header,  |                       |
|                       | since the host name   |                       |
|                       | and/or port of the    |                       |
|                       | reverse proxy (load   |                       |
|                       | balancer) may differ  |                       |
|                       | from the origin       |                       |
|                       | server handling the   |                       |
|                       | request. Superseded   |                       |
|                       | by *Forwarded*        |                       |
|                       | header.               |                       |
+-----------------------+-----------------------+-----------------------+
| X-Forwarded-Proto[^52 | A [*de facto*         | `X-Forwarded-Proto: h |
| ]                     | standard](de_facto_st | ttps`                 |
|                       | andard "wikilink")    |                       |
|                       | for identifying the   |                       |
|                       | originating protocol  |                       |
|                       | of an HTTP request,   |                       |
|                       | since a reverse proxy |                       |
|                       | (or a load balancer)  |                       |
|                       | may communicate with  |                       |
|                       | a web server using    |                       |
|                       | HTTP even if the      |                       |
|                       | request to the        |                       |
|                       | reverse proxy is      |                       |
|                       | HTTPS. An alternative |                       |
|                       | form of the header    |                       |
|                       | (X-ProxyUser-Ip) is   |                       |
|                       | used by Google        |                       |
|                       | clients talking to    |                       |
|                       | Google servers.       |                       |
|                       | Superseded by         |                       |
|                       | *Forwarded* header.   |                       |
+-----------------------+-----------------------+-----------------------+
| Front-End-Https[^53]  | Non-standard header   | `Front-End-Https: on` |
|                       | field used by         |                       |
|                       | Microsoft             |                       |
|                       | applications and      |                       |
|                       | load-balancers        |                       |
+-----------------------+-----------------------+-----------------------+
| X-Http-Method-Overrid | Requests a web        | `X-HTTP-Method-Overri |
| e[^54]                | application to        | de: DELETE`           |
|                       | override the method   |                       |
|                       | specified in the      |                       |
|                       | request (typically    |                       |
|                       | POST) with the method |                       |
|                       | given in the header   |                       |
|                       | field (typically PUT  |                       |
|                       | or DELETE). This can  |                       |
|                       | be used when a user   |                       |
|                       | agent or firewall     |                       |
|                       | prevents PUT or       |                       |
|                       | DELETE methods from   |                       |
|                       | being sent directly   |                       |
|                       | (note that this is    |                       |
|                       | either a bug in the   |                       |
|                       | software component,   |                       |
|                       | which ought to be     |                       |
|                       | fixed, or an          |                       |
|                       | intentional           |                       |
|                       | configuration, in     |                       |
|                       | which case bypassing  |                       |
|                       | it may be the wrong   |                       |
|                       | thing to do).         |                       |
+-----------------------+-----------------------+-----------------------+
| X-ATT-DeviceId[^55]   | Allows easier parsing | `X-Att-Deviceid: GT-P |
|                       | of the                | 7320/P7320XXLPG`      |
|                       | MakeModel/Firmware    |                       |
|                       | that is usually found |                       |
|                       | in the User-Agent     |                       |
|                       | String of AT&T        |                       |
|                       | Devices               |                       |
+-----------------------+-----------------------+-----------------------+
| X-Wap-Profile[^56]    | Links to an XML file  | `x-wap-profile: `[`ht |
|                       | on the Internet with  | tp://wap.samsungmobil |
|                       | a full description    | e.com/uaprof/SGH-I777 |
|                       | and details about the | .xml`](http://wap.sam |
|                       | device currently      | sungmobile.com/uaprof |
|                       | connecting. In the    | /SGH-I777.xml)        |
|                       | example to the right  |                       |
|                       | is an XML file for an |                       |
|                       | AT&T Samsung Galaxy   |                       |
|                       | S2.                   |                       |
+-----------------------+-----------------------+-----------------------+
| Proxy-Connection[^57] | Implemented as a      | `Proxy-Connection: ke |
|                       | misunderstanding of   | ep-alive`             |
|                       | the HTTP              |                       |
|                       | specifications.       |                       |
|                       | Common because of     |                       |
|                       | mistakes in           |                       |
|                       | implementations of    |                       |
|                       | early HTTP versions.  |                       |
|                       | Has exactly the same  |                       |
|                       | functionality as      |                       |
|                       | standard Connection   |                       |
|                       | field. Must not be    |                       |
|                       | used with             |                       |
|                       | HTTP/2.[^58]          |                       |
+-----------------------+-----------------------+-----------------------+
| X-UIDH[^59][^60][^61] | Server-side [deep     | `X-UIDH: ...`         |
|                       | packet                |                       |
|                       | insertion](Deep_packe |                       |
|                       | t_inspection "wikilin |                       |
|                       | k")                   |                       |
|                       | of a unique ID        |                       |
|                       | identifying customers |                       |
|                       | of [Verizon           |                       |
|                       | Wireless](Verizon_Wir |                       |
|                       | eless "wikilink");    |                       |
|                       | also known as         |                       |
|                       | \"perma-cookie\" or   |                       |
|                       | \"supercookie\"       |                       |
+-----------------------+-----------------------+-----------------------+
| X-Csrf-Token[^62]     | Used to prevent       | `X-Csrf-Token: i8XNjC |
|                       | [cross-site request   | 4b8KVok4uw5RftR38Wgp2 |
|                       | forgery](cross-site_r | BFwql`                |
|                       | equest_forgery "wikil |                       |
|                       | ink").                |                       |
|                       | Alternative header    |                       |
|                       | names are:            |                       |
|                       | `X-CSRFToken`[^63]    |                       |
|                       | and                   |                       |
|                       | `X-XSRF-TOKEN`[^64]   |                       |
+-----------------------+-----------------------+-----------------------+
| X-Request-ID[^65][^66 | Correlates HTTP       | `X-Request-ID: f058eb |
| ],                    | requests between a    | d6-02f7-4d3f-942e-904 |
| X-Correlation-ID[^67] | client and server.    | 344e8cde5`            |
| [^68]                 |                       |                       |
+-----------------------+-----------------------+-----------------------+
| Save-Data             | The Save-Data client  | `Save-Data: on`       |
|                       | hint request header   |                       |
|                       | available in Chrome,  |                       |
|                       | Opera, and Yandex     |                       |
|                       | browsers lets         |                       |
|                       | developers deliver    |                       |
|                       | lighter, faster       |                       |
|                       | applications to users |                       |
|                       | who opt-in to data    |                       |
|                       | saving mode in their  |                       |
|                       | browser.              |                       |
+-----------------------+-----------------------+-----------------------+
```