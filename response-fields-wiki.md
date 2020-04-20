Response fields {#response_fields}
---------------

### Standard response fields {#standard_response_fields}

+-------------+-------------+-------------+-------------+-------------+
| Field name  | Description | Example     | Status      | Standard    |
+=============+=============+=============+=============+=============+
| ```{=mediaw | Specifying  | `Access-Con | ```{=mediaw |             |
| iki}        | which web   | trol-Allow- | iki}        |             |
| {{nowrap|Ac | sites can   | Origin: *`  | {{nowrap|Pe |             |
| cess-Contro | participate |             | rmanent: st |             |
| l-Allow-Ori | in          |             | andard}}    |             |
| gin,<br/>Ac | [cross-orig |             | ```         |             |
| cess-Contro | in          |             |             |             |
| l-Allow-Cre | resource    |             |             |             |
| dentials,<b | sharing](cr |             |             |             |
| r />Access- | oss-origin_ |             |             |             |
| Control-Exp | resource_sh |             |             |             |
| ose-Headers | aring "wiki |             |             |             |
| ,<br />Acce | link")      |             |             |             |
| ss-Control- |             |             |             |             |
| Max-Age,<br |             |             |             |             |
|  />Access-C |             |             |             |             |
| ontrol-Allo |             |             |             |             |
| w-Methods,< |             |             |             |             |
| br />Access |             |             |             |             |
| -Control-Al |             |             |             |             |
| low-Headers |             |             |             |             |
| }}          |             |             |             |             |
| ```         |             |             |             |             |
| [^19]       |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Accept-Patc | Specifies   | `Accept-Pat | Permanent   |             |
| h[^20]      | which patch | ch: text/ex |             |             |
|             | document    | ample;chars |             |             |
|             | formats     | et=utf-8`   |             |             |
|             | this server |             |             |             |
|             | supports    |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Accept-Rang | What        | `Accept-Ran | Permanent   |             |
| es          | partial     | ges: bytes` |             |             |
|             | content     |             |             |             |
|             | range types |             |             |             |
|             | this server |             |             |             |
|             | supports    |             |             |             |
|             | via [byte   |             |             |             |
|             | serving](by |             |             |             |
|             | te_serving  |             |             |             |
|             | "wikilink") |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Age         | The age the | `Age: 12`   | Permanent   |             |
|             | object has  |             |             |             |
|             | been in a   |             |             |             |
|             | [proxy      |             |             |             |
|             | cache](prox |             |             |             |
|             | y_cache "wi |             |             |             |
|             | kilink")    |             |             |             |
|             | in seconds  |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Allow       | Valid       | `Allow: GET | Permanent   |             |
|             | methods for | , HEAD`     |             |             |
|             | a specified |             |             |             |
|             | resource.   |             |             |             |
|             | To be used  |             |             |             |
|             | for a *405  |             |             |             |
|             | Method not  |             |             |             |
|             | allowed*    |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Alt-Svc<ref | date=April  | A server    | date=April  | `Alt-Svc: h |
| >{{cite     | 2016\|acces | uses        | 2016\|acces | ttp/1.1="ht |
| web\|url=<h | sdate=2016- | \"Alt-Svc\" | sdate=2017- | tp2.example |
| ttps://tool | 04-19}}</re | header      | 06-08}}</re | .com:8001"; |
| s.ietf.org/ | f>          | (meaning    | f>          |  ma=7200`   |
| html/rfc783 |             | Alternative |             |             |
| 8%7Ctitle=H |             | Services)   |             |             |
| TTP>        |             | to indicate |             |             |
| Alternative |             | that its    |             |             |
| Services    |             | resources   |             |             |
|             |             | can also be |             |             |
|             |             | accessed at |             |             |
|             |             | a different |             |             |
|             |             | network     |             |             |
|             |             | location    |             |             |
|             |             | (host or    |             |             |
|             |             | port) or    |             |             |
|             |             | using a     |             |             |
|             |             | different   |             |             |
|             |             | protocol    |             |             |
|             |             |             |             |             |
|             |             | When using  |             |             |
|             |             | HTTP/2,     |             |             |
|             |             | servers     |             |             |
|             |             | should      |             |             |
|             |             | instead     |             |             |
|             |             | send an     |             |             |
|             |             | ALTSVC      |             |             |
|             |             | frame.      |             |             |
|             |             | <ref>{{cite |             |             |
|             |             | web\|url=<h |             |             |
|             |             | ttps://tool |             |             |
|             |             | s.ietf.org/ |             |             |
|             |             | html/rfc783 |             |             |
|             |             | 8#section-3 |             |             |
|             |             | %7Ctitle=HT |             |             |
|             |             | TP>         |             |             |
|             |             | Alternative |             |             |
|             |             | Services,   |             |             |
|             |             | section 3   |             |             |
+-------------+-------------+-------------+-------------+-------------+
| [Cache-Cont | Tells all   | `Cache-Cont | Permanent   |             |
| rol](Cache- | caching     | rol: max-ag |             |             |
| Control "wi | mechanisms  | e=3600`     |             |             |
| kilink")    | from server |             |             |             |
|             | to client   |             |             |             |
|             | whether     |             |             |             |
|             | they may    |             |             |             |
|             | cache this  |             |             |             |
|             | object. It  |             |             |             |
|             | is measured |             |             |             |
|             | in seconds  |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Connection  | Control     | `Connection | Permanent   |             |
|             | options for | : close`    |             |             |
|             | the current |             |             |             |
|             | connection  |             |             |             |
|             | and list of |             |             |             |
|             | hop-by-hop  |             |             |             |
|             | response    |             |             |             |
|             | fields.[^21 |             |             |             |
|             | ]           |             |             |             |
|             | Must not be |             |             |             |
|             | used with   |             |             |             |
|             | HTTP/2.[^22 |             |             |             |
|             | ]           |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Content-Dis | An          | `Content-Di | Permanent   |             |
| position[^2 | opportunity | sposition:  |             |             |
| 3]          | to raise a  | attachment; |             |             |
|             | \"File      |  filename=" |             |             |
|             | Download\"  | fname.ext"` |             |             |
|             | dialogue    |             |             |             |
|             | box for a   |             |             |             |
|             | known MIME  |             |             |             |
|             | type with   |             |             |             |
|             | binary      |             |             |             |
|             | format or   |             |             |             |
|             | suggest a   |             |             |             |
|             | filename    |             |             |             |
|             | for dynamic |             |             |             |
|             | content.    |             |             |             |
|             | Quotes are  |             |             |             |
|             | necessary   |             |             |             |
|             | with        |             |             |             |
|             | special     |             |             |             |
|             | characters. |             |             |             |
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
| Content-Lan | The natural | `Content-La | Permanent   |             |
| guage       | language or | nguage: da` |             |             |
|             | languages   |             |             |             |
|             | of the      |             |             |             |
|             | intended    |             |             |             |
|             | audience    |             |             |             |
|             | for the     |             |             |             |
|             | enclosed    |             |             |             |
|             | content[^24 |             |             |             |
|             | ]           |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Content-Len | The length  | `Content-Le | Permanent   |             |
| gth         | of the      | ngth: 348`  |             |             |
|             | response    |             |             |             |
|             | body in     |             |             |             |
|             | [octets](Oc |             |             |             |
|             | tet_(comput |             |             |             |
|             | ing) "wikil |             |             |             |
|             | ink")       |             |             |             |
|             | (8-bit      |             |             |             |
|             | bytes)      |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Content-Loc | An          | `Content-Lo | Permanent   |             |
| ation       | alternate   | cation: /in |             |             |
|             | location    | dex.htm`    |             |             |
|             | for the     |             |             |             |
|             | returned    |             |             |             |
|             | data        |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Content-MD5 | A           | `Content-MD | Obsolete[^2 |             |
|             | [Base64](Ba | 5: Q2hlY2sg | 5]          |             |
|             | se64 "wikil | SW50ZWdyaXR |             |             |
|             | ink")-encod | 5IQ==`      |             |             |
|             | ed          |             |             |             |
|             | binary      |             |             |             |
|             | [MD5](MD5 " |             |             |             |
|             | wikilink")  |             |             |             |
|             | sum of the  |             |             |             |
|             | content of  |             |             |             |
|             | the         |             |             |             |
|             | response    |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Content-Ran | Where in a  | `Content-Ra | Permanent   |             |
| ge          | full body   | nge: bytes  |             |             |
|             | message     | 21010-47021 |             |             |
|             | this        | /47022`     |             |             |
|             | partial     |             |             |             |
|             | message     |             |             |             |
|             | belongs     |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Content-Typ | The [MIME   | `Content-Ty | Permanent   |             |
| e           | type](MIME_ | pe: text/ht |             |             |
|             | type "wikil | ml; charset |             |             |
|             | ink")       | =utf-8`     |             |             |
|             | of this     |             |             |             |
|             | content     |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Date        | The date    | `Date: Tue, | Permanent   |             |
|             | and time    |  15 Nov 199 |             |             |
|             | that the    | 4 08:12:31  |             |             |
|             | message was | GMT`        |             |             |
|             | sent (in    |             |             |             |
|             | \"HTTP-date |             |             |             |
|             | \"          |             |             |             |
|             | format as   |             |             |             |
|             | defined by  |             |             |             |
|             | RFC 7231)   |             |             |             |
|             | [^26]       |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Delta-Base  | Specifies   | `Delta-Base | Permanent   |             |
|             | the         | : "abc"`    |             |             |
|             | delta-encod |             |             |             |
|             | ing         |             |             |             |
|             | entity tag  |             |             |             |
|             | of the      |             |             |             |
|             | response.[^ |             |             |             |
|             | 27]         |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| [ETag](HTTP | An          | `ETag: "737 | Permanent   |             |
| _ETag "wiki | identifier  | 060cd8c284d |             |             |
| link")      | for a       | 8af7ad3082f |             |             |
|             | specific    | 209582d"`   |             |             |
|             | version of  |             |             |             |
|             | a resource, |             |             |             |
|             | often a     |             |             |             |
|             | [message    |             |             |             |
|             | digest](mes |             |             |             |
|             | sage_digest |             |             |             |
|             |  "wikilink" |             |             |             |
|             | )           |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Expires     | Gives the   | `Expires: T | Permanent:  |             |
|             | date/time   | hu, 01 Dec  | standard    |             |
|             | after which | 1994 16:00: |             |             |
|             | the         | 00 GMT`     |             |             |
|             | response is |             |             |             |
|             | considered  |             |             |             |
|             | stale (in   |             |             |             |
|             | \"HTTP-date |             |             |             |
|             | \"          |             |             |             |
|             | format as   |             |             |             |
|             | defined by  |             |             |             |
|             | RFC 7231)   |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| IM          | Instance-ma | `IM: feed`  | Permanent   |             |
|             | nipulations |             |             |             |
|             | applied to  |             |             |             |
|             | the         |             |             |             |
|             | response.[^ |             |             |             |
|             | 28]         |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Last-Modifi | The last    | `Last-Modif | Permanent   |             |
| ed          | modified    | ied: Tue, 1 |             |             |
|             | date for    | 5 Nov 1994  |             |             |
|             | the         | 12:45:26 GM |             |             |
|             | requested   | T`          |             |             |
|             | object (in  |             |             |             |
|             | \"HTTP-date |             |             |             |
|             | \"          |             |             |             |
|             | format as   |             |             |             |
|             | defined by  |             |             |             |
|             | RFC 7231)   |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Link        | Used to     | `Link: </fe | Permanent   |             |
|             | express a   | ed>; rel="a |             |             |
|             | typed       | lternate"`[ |             |             |
|             | relationshi | ^29]        |             |             |
|             | p           |             |             |             |
|             | with        |             |             |             |
|             | another     |             |             |             |
|             | resource,   |             |             |             |
|             | where the   |             |             |             |
|             | relation    |             |             |             |
|             | type is     |             |             |             |
|             | defined by  |             |             |             |
|             | RFC 5988    |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| [Location]( | Used in     | -   Example | Permanent   |             |
| HTTP_locati | [redirectio |     1:      |             |             |
| on "wikilin | n](URL_redi |     `Locati |             |             |
| k")         | rection "wi | on: http:// |             |             |
|             | kilink"),   | www.w3.org/ |             |             |
|             | or when a   | pub/WWW/Peo |             |             |
|             | new         | ple.html`   |             |             |
|             | resource    | -   Example |             |             |
|             | has been    |     2:      |             |             |
|             | created.    |     `Locati |             |             |
|             |             | on: /pub/WW |             |             |
|             |             | W/People.ht |             |             |
|             |             | ml`         |             |             |
+-------------+-------------+-------------+-------------+-------------+
| [P3P](P3P " | This field  | `P3P: CP="T | Permanent   |             |
| wikilink")  | is supposed | his is not  |             |             |
|             | to set      | a P3P polic |             |             |
|             | [P3P](P3P " | y! See http |             |             |
|             | wikilink")  | s://en.wiki |             |             |
|             | policy, in  | pedia.org/w |             |             |
|             | the form of | iki/Special |             |             |
|             | `P3P:CP="yo | :CentralAut |             |             |
|             | ur_compact_ | oLogin/P3P  |             |             |
|             | policy"`.   | for more in |             |             |
|             | However,    | fo."`       |             |             |
|             | P3P did not |             |             |             |
|             | take        |             |             |             |
|             | off,[^30]   |             |             |             |
|             | most        |             |             |             |
|             | browsers    |             |             |             |
|             | have never  |             |             |             |
|             | fully       |             |             |             |
|             | implemented |             |             |             |
|             | it, a lot   |             |             |             |
|             | of websites |             |             |             |
|             | set this    |             |             |             |
|             | field with  |             |             |             |
|             | fake policy |             |             |             |
|             | text, that  |             |             |             |
|             | was enough  |             |             |             |
|             | to fool     |             |             |             |
|             | browsers    |             |             |             |
|             | the         |             |             |             |
|             | existence   |             |             |             |
|             | of P3P      |             |             |             |
|             | policy and  |             |             |             |
|             | grant       |             |             |             |
|             | permissions |             |             |             |
|             | for [third  |             |             |             |
|             | party       |             |             |             |
|             | cookies](Th |             |             |             |
|             | ird_party_c |             |             |             |
|             | ookie "wiki |             |             |             |
|             | link").     |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Pragma      | Implementat | `Pragma: no | Permanent   |             |
|             | ion-specifi | -cache`     |             |             |
|             | c           |             |             |             |
|             | fields that |             |             |             |
|             | may have    |             |             |             |
|             | various     |             |             |             |
|             | effects     |             |             |             |
|             | anywhere    |             |             |             |
|             | along the   |             |             |             |
|             | request-res |             |             |             |
|             | ponse       |             |             |             |
|             | chain.      |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Proxy-Authe | Request     | `Proxy-Auth | Permanent   |             |
| nticate     | authenticat | enticate: B |             |             |
|             | ion         | asic`       |             |             |
|             | to access   |             |             |             |
|             | the proxy.  |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Public-Key- | [HTTP       | `Public-Key | Permanent   |             |
| Pins[^31]   | Public Key  | -Pins: max- |             |             |
|             | Pinning](HT | age=2592000 |             |             |
|             | TP_Public_K | ; pin-sha25 |             |             |
|             | ey_Pinning  | 6="E9CZ9IND |             |             |
|             | "wikilink") | bd+2eRQozYq |             |             |
|             | ,           | qbQ2yXLVKB9 |             |             |
|             | announces   | +xcprMF+44U |             |             |
|             | hash of     | 1g=";`      |             |             |
|             | website\'s  |             |             |             |
|             | authentic   |             |             |             |
|             | [TLS](Trans |             |             |             |
|             | port_Layer_ |             |             |             |
|             | Security "w |             |             |             |
|             | ikilink")   |             |             |             |
|             | certificate |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Retry-After | If an       | -   Example | Permanent   |             |
|             | entity is   |     1:      |             |             |
|             | temporarily |     `Retry- |             |             |
|             | unavailable | After: 120` |             |             |
|             | ,           | -   Example |             |             |
|             | this        |     2:      |             |             |
|             | instructs   |     `Retry- |             |             |
|             | the client  | After: Fri, |             |             |
|             | to try      |  07 Nov 201 |             |             |
|             | again       | 4 23:59:59  |             |             |
|             | later.      | GMT`        |             |             |
|             | Value could |             |             |             |
|             | be a        |             |             |             |
|             | specified   |             |             |             |
|             | period of   |             |             |             |
|             | time (in    |             |             |             |
|             | seconds) or |             |             |             |
|             | a           |             |             |             |
|             | HTTP-date.[ |             |             |             |
|             | ^32]        |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Server      | A name for  | `Server: Ap | Permanent   |             |
|             | the server  | ache/2.4.1  |             |             |
|             |             | (Unix)`     |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Set-Cookie  | An [HTTP    | `Set-Cookie | Permanent:  |             |
|             | cookie](HTT | : UserID=Jo | standard    |             |
|             | P_cookie "w | hnDoe; Max- |             |             |
|             | ikilink")   | Age=3600; V |             |             |
|             |             | ersion=1`   |             |             |
+-------------+-------------+-------------+-------------+-------------+
| [Strict-Tra | A HSTS      | `Strict-Tra | Permanent:  |             |
| nsport-Secu | Policy      | nsport-Secu | standard    |             |
| rity](HTTP_ | informing   | rity: max-a |             |             |
| Strict_Tran | the HTTP    | ge=16070400 |             |             |
| sport_Secur | client how  | ; includeSu |             |             |
| ity "wikili | long to     | bDomains`   |             |             |
| nk")        | cache the   |             |             |             |
|             | HTTPS only  |             |             |             |
|             | policy and  |             |             |             |
|             | whether     |             |             |             |
|             | this        |             |             |             |
|             | applies to  |             |             |             |
|             | subdomains. |             |             |             |
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
|             | HTTP/2.[^33 |             |             |             |
|             | ]           |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Tk          | Tracking    | `Tk: ?`     | Permanent   |             |
|             | Status      |             |             |             |
|             | header,     |             |             |             |
|             | value       |             |             |             |
|             | suggested   |             |             |             |
|             | to be sent  |             |             |             |
|             | in response |             |             |             |
|             | to a        |             |             |             |
|             | DNT(do-not- |             |             |             |
|             | track),     |             |             |             |
|             | possible    |             |             |             |
|             | values:     |             |             |             |
|             |             |             |             |             |
|             | `"!" — unde |             |             |             |
|             | r construct |             |             |             |
|             | ion`\       |             |             |             |
|             | `"?" — dyna |             |             |             |
|             | mic`\       |             |             |             |
|             | `"G" — gate |             |             |             |
|             | way to mult |             |             |             |
|             | iple partie |             |             |             |
|             | s`\         |             |             |             |
|             | `"N" — not  |             |             |             |
|             | tracking`\  |             |             |             |
|             | `"T" — trac |             |             |             |
|             | king`\      |             |             |             |
|             | `"C" — trac |             |             |             |
|             | king with c |             |             |             |
|             | onsent`\    |             |             |             |
|             | `"P" — trac |             |             |             |
|             | king only i |             |             |             |
|             | f consented |             |             |             |
|             | `\          |             |             |             |
|             | `"D" — disr |             |             |             |
|             | egarding DN |             |             |             |
|             | T`\         |             |             |             |
|             | `"U" — upda |             |             |             |
|             | ted`        |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| [Upgrade](U | Ask the     | `Upgrade: h | Permanent   |             |
| pgrade_head | client to   | 2c, HTTPS/1 |             |             |
| er "wikilin | upgrade to  | .3, IRC/6.9 |             |             |
| k")         | another     | , RTA/x11,  |             |             |
|             | protocol.   | websocket`  |             |             |
|             | Must not be |             |             |             |
|             | used in     |             |             |             |
|             | HTTP/2[^34] |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Vary        | Tells       | -   Example | Permanent   |             |
|             | downstream  |     1:      |             |             |
|             | proxies how |     `Vary:  |             |             |
|             | to match    | *`          |             |             |
|             | future      | -   Example |             |             |
|             | request     |     2:      |             |             |
|             | headers to  |     `Vary:  |             |             |
|             | decide      | Accept-Lang |             |             |
|             | whether the | uage`       |             |             |
|             | cached      |             |             |             |
|             | response    |             |             |             |
|             | can be used |             |             |             |
|             | rather than |             |             |             |
|             | requesting  |             |             |             |
|             | a fresh one |             |             |             |
|             | from the    |             |             |             |
|             | origin      |             |             |             |
|             | server.     |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Via         | Informs the | `Via: 1.0 f | Permanent   |             |
|             | client of   | red, 1.1 ex |             |             |
|             | proxies     | ample.com ( |             |             |
|             | through     | Apache/1.1) |             |             |
|             | which the   | `           |             |             |
|             | response    |             |             |             |
|             | was sent.   |             |             |             |
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
| WWW-Authent | Indicates   | `WWW-Authen | Permanent   |             |
| icate       | the         | ticate: Bas |             |             |
|             | authenticat | ic`         |             |             |
|             | ion         |             |             |             |
|             | scheme that |             |             |             |
|             | should be   |             |             |             |
|             | used to     |             |             |             |
|             | access the  |             |             |             |
|             | requested   |             |             |             |
|             | entity.     |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| X-Frame-Opt | [Clickjacki | `X-Frame-Op | Obsolete[^3 |             |
| ions[^35]   | ng](Clickja | tions: deny | 6]          |             |
|             | cking "wiki | `           |             |             |
|             | link")      |             |             |             |
|             | protection: |             |             |             |
|             | `deny` - no |             |             |             |
|             | rendering   |             |             |             |
|             | within a    |             |             |             |
|             | frame,      |             |             |             |
|             | `sameorigin |             |             |             |
|             | `           |             |             |             |
|             | - no        |             |             |             |
|             | rendering   |             |             |             |
|             | if origin   |             |             |             |
|             | mismatch,   |             |             |             |
|             | `allow-from |             |             |             |
|             | `           |             |             |             |
|             | - allow     |             |             |             |
|             | from        |             |             |             |
|             | specified   |             |             |             |
|             | location,   |             |             |             |
|             | `allowall`  |             |             |             |
|             | -           |             |             |             |
|             | non-standar |             |             |             |
|             | d,          |             |             |             |
|             | allow from  |             |             |             |
|             | any         |             |             |             |
|             | location    |             |             |             |
+-------------+-------------+-------------+-------------+-------------+

### Common non-standard response fields {#common_non_standard_response_fields}

+-----------------------+-----------------------+-----------------------+
| Field name            | Description           | Example               |
+=======================+=======================+=======================+
| Content-Security-Poli | [Content Security     | `X-WebKit-CSP: defaul |
| cy,\                  | Policy](Content_Secur | t-src 'self'`         |
| X-Content-Security-Po | ity_Policy "wikilink" |                       |
| licy,\                | )                     |                       |
| X-WebKit-CSP[^48]     | definition.           |                       |
+-----------------------+-----------------------+-----------------------+
| [Refresh](HTTP_refres | Used in redirection,  | `Refresh: 5; url=http |
| h "wikilink")         | or when a new         | ://www.w3.org/pub/WWW |
|                       | resource has been     | /People.html`         |
|                       | created. This refresh |                       |
|                       | redirects after 5     |                       |
|                       | seconds. Header       |                       |
|                       | extension introduced  |                       |
|                       | by Netscape and       |                       |
|                       | supported by most web |                       |
|                       | browsers.             |                       |
+-----------------------+-----------------------+-----------------------+
| Status                | [CGI](Common_Gateway_ | `Status: 200 OK`      |
|                       | Interface "wikilink") |                       |
|                       | header field          |                       |
|                       | specifying the        |                       |
|                       | [status](HTTP_status  |                       |
|                       | "wikilink")           |                       |
|                       | of the HTTP response. |                       |
|                       | Normal HTTP responses |                       |
|                       | use a separate        |                       |
|                       | \"Status-Line\"       |                       |
|                       | instead, defined by   |                       |
|                       | RFC 7230.[^49]        |                       |
+-----------------------+-----------------------+-----------------------+
| Timing-Allow-Origin   | The                   | `Timing-Allow-Origin: |
|                       | `Timing-Allow-Origin` |  *`                   |
|                       | response header       | `Timing-Allow-Origin: |
|                       | specifies origins     |  `<origin>`[, `<origi |
|                       | that are allowed to   | n>`]*`                |
|                       | see values of         |                       |
|                       | attributes retrieved  |                       |
|                       | via features of the   |                       |
|                       | [Resource Timing      |                       |
|                       | API](https://develope |                       |
|                       | r.mozilla.org/en-US/d |                       |
|                       | ocs/Web/API/Resource_ |                       |
|                       | Timing_API),          |                       |
|                       | which would otherwise |                       |
|                       | be reported as zero   |                       |
|                       | due to cross-origin   |                       |
|                       | restrictions.[^50]    |                       |
+-----------------------+-----------------------+-----------------------+
| X-Content-Duration[^5 | Provide the duration  | `X-Content-Duration:  |
| 1]                    | of the audio or video | 42.666`               |
|                       | in seconds; only      |                       |
|                       | supported by Gecko    |                       |
|                       | browsers              |                       |
+-----------------------+-----------------------+-----------------------+
| X-Content-Type-Option | The only defined      | `X-Content-Type-Optio |
| s[^52]                | value, \"nosniff\",   | ns: nosniff`[^54]     |
|                       | prevents [Internet    |                       |
|                       | Explorer](Internet_Ex |                       |
|                       | plorer "wikilink")    |                       |
|                       | from MIME-sniffing a  |                       |
|                       | response away from    |                       |
|                       | the declared          |                       |
|                       | content-type. This    |                       |
|                       | also applies to       |                       |
|                       | [Google               |                       |
|                       | Chrome](Google_Chrome |                       |
|                       |  "wikilink"),         |                       |
|                       | when downloading      |                       |
|                       | extensions.[^53]      |                       |
+-----------------------+-----------------------+-----------------------+
| X-Powered-By[^55]     | Specifies the         | `X-Powered-By: PHP/5. |
|                       | technology (e.g.      | 4.0`                  |
|                       | ASP.NET, PHP, JBoss)  |                       |
|                       | supporting the web    |                       |
|                       | application (version  |                       |
|                       | details are often in  |                       |
|                       | `X-Runtime`,          |                       |
|                       | `X-Version`, or       |                       |
|                       | `X-AspNet-Version`)   |                       |
+-----------------------+-----------------------+-----------------------+
| X-Request-ID,\        | Correlates HTTP       | `X-Request-ID: f058eb |
| X-Correlation-ID[^56] | requests between a    | d6-02f7-4d3f-942e-904 |
|                       | client and server.    | 344e8cde5`            |
+-----------------------+-----------------------+-----------------------+
| X-UA-Compatible[^57]  | Recommends the        | `X-UA-Compatible: IE= |
|                       | preferred rendering   | EmulateIE7`\          |
|                       | engine (often a       | `X-UA-Compatible: IE= |
|                       | backward-compatibilit | edge`\                |
|                       | y                     | `X-UA-Compatible: Chr |
|                       | mode) to use to       | ome=1`                |
|                       | display the content.  |                       |
|                       | Also used to activate |                       |
|                       | [Chrome               |                       |
|                       | Frame](Chrome_Frame " |                       |
|                       | wikilink")            |                       |
|                       | in Internet Explorer. |                       |
+-----------------------+-----------------------+-----------------------+
| X-XSS-Protection[^58] | [Cross-site           | `X-XSS-Protection: 1; |
|                       | scripting](Cross-site |  mode=block`          |
|                       | _scripting "wikilink" |                       |
|                       | )                     |                       |
|                       | (XSS) filter          |                       |
+-----------------------+-----------------------+-----------------------+

[^1]: 

[^2]: `{{cite web|url=http://tools.ietf.org/html/rfc5789#section-3.1 |title=RFC 5789 |accessdate=2014-12-24}}`{=mediawiki}

[^3]: 

[^4]: 

[^5]: `{{cite web|url=http://tools.ietf.org/html/rfc6266 |title=RFC 6266 |accessdate=2015-03-13}}`{=mediawiki}

[^6]: `{{cite web|url=https://tools.ietf.org/html/rfc7231#section-3.1.3.2 |title=RFC 7231 - Hypertext Transfer Protocol (HTTP/1.1): Semantics and Content |publisher=Tools.ietf.org |date= |accessdate=2017-12-11}}`{=mediawiki}

[^7]: 

[^8]: `{{cite web|url=http://ronwilliams.io/blog/post/rfc7231-compliant-http-date-headers |title=RFC7231 Compliant HTTP Date Headers}}`{=mediawiki}

[^9]: 

[^10]: 

[^11]: [Indicate the canonical version of a URL by responding with the
    Link rel=\"canonical\" HTTP
    header](https://support.google.com/webmasters/bin/answer.py?hl=en&answer=139394)
    Retrieved: 2012-02-09

[^12]: W3C [P3P Work Suspended](http://www.w3.org/P3P)

[^13]: `{{cite web | url=http://www.rfc-editor.org/rfc/rfc7469.txt | title=Public Key Pinning Extension for HTTP | publisher=IETF | accessdate=17 April 2015}}`{=mediawiki}

[^14]: `{{cite web|url=http://tools.ietf.org/html/rfc7231#section-7.1.3|title=Hypertext Transfer Protocol (HTTP/1.1): Semantics and Content|accessdate=2014-07-24}}`{=mediawiki}

[^15]: 

[^16]: 

[^17]: `{{cite web|url=https://tools.ietf.org/html/rfc7034|title=HTTP Header Field X-Frame-Options |year=2013 |publisher=IETF |accessdate=2014-06-12}}`{=mediawiki}

[^18]: `{{cite web|url=http://www.w3.org/TR/CSP11/#frame-ancestors-and-frame-options |title=Content Security Policy Level 2 |accessdate=2014-08-02}}`{=mediawiki}

[^19]: 

[^20]: `{{cite web|url=http://tools.ietf.org/html/rfc5789#section-3.1 |title=RFC 5789 |accessdate=2014-12-24}}`{=mediawiki}

[^21]: 

[^22]: 

[^23]: `{{cite web|url=http://tools.ietf.org/html/rfc6266 |title=RFC 6266 |accessdate=2015-03-13}}`{=mediawiki}

[^24]: `{{cite web|url=https://tools.ietf.org/html/rfc7231#section-3.1.3.2 |title=RFC 7231 - Hypertext Transfer Protocol (HTTP/1.1): Semantics and Content |publisher=Tools.ietf.org |date= |accessdate=2017-12-11}}`{=mediawiki}

[^25]: 

[^26]: `{{cite web|url=http://ronwilliams.io/blog/post/rfc7231-compliant-http-date-headers |title=RFC7231 Compliant HTTP Date Headers}}`{=mediawiki}

[^27]: 

[^28]: 

[^29]: [Indicate the canonical version of a URL by responding with the
    Link rel=\"canonical\" HTTP
    header](https://support.google.com/webmasters/bin/answer.py?hl=en&answer=139394)
    Retrieved: 2012-02-09

[^30]: W3C [P3P Work Suspended](http://www.w3.org/P3P)

[^31]: `{{cite web | url=http://www.rfc-editor.org/rfc/rfc7469.txt | title=Public Key Pinning Extension for HTTP | publisher=IETF | accessdate=17 April 2015}}`{=mediawiki}

[^32]: `{{cite web|url=http://tools.ietf.org/html/rfc7231#section-7.1.3|title=Hypertext Transfer Protocol (HTTP/1.1): Semantics and Content|accessdate=2014-07-24}}`{=mediawiki}

[^33]: 

[^34]: 

[^35]: `{{cite web|url=https://tools.ietf.org/html/rfc7034|title=HTTP Header Field X-Frame-Options |year=2013 |publisher=IETF |accessdate=2014-06-12}}`{=mediawiki}

[^36]: `{{cite web|url=http://www.w3.org/TR/CSP11/#frame-ancestors-and-frame-options |title=Content Security Policy Level 2 |accessdate=2014-08-02}}`{=mediawiki}

[^37]: `{{cite web|url=http://www.w3.org/TR/CSP/|title=Content Security Policy |publisher=W3C |year=2012|accessdate=28 April 2017}}`{=mediawiki}

[^38]: `{{cite web|url=http://tools.ietf.org/html/rfc7230#section-3.1.2|title=Hypertext Transfer Protocol (HTTP/1.1): Message Syntax and Routing|accessdate=2014-07-24}}`{=mediawiki}

[^39]: `{{Cite web|url=https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Timing-Allow-Origin|title=Timing-Allow-Origin|website=Mozilla Developer Network|language=en-US|access-date=2018-01-25}}`{=mediawiki}

[^40]: `{{cite web|url=https://developer.mozilla.org/en-US/docs/Web/HTTP/Configuring_servers_for_Ogg_media#Serve_X-Content-Duration_headers |title=Configuring servers for Ogg media |date=2014-05-26 |accessdate=2015-01-03}}`{=mediawiki}

[^41]: `{{cite web|url=http://blogs.msdn.com/b/ie/archive/2008/09/02/ie8-security-part-vi-beta-2-update.aspx |title=IE8 Security Part VI: Beta 2 Update |author=Eric Lawrence |date=2008-09-03 |accessdate=2010-09-28}}`{=mediawiki}

[^42]: `{{cite web|url=https://code.google.com/chrome/extensions/hosting.html |title=Hosting - Google Chrome Extensions - Google Code |accessdate=2012-06-14}}`{=mediawiki}

[^43]: `{{cite web |url=https://fetch.spec.whatwg.org/#x-content-type-options-header |title=Fetch standard |last1=van Kesteren |first1=Anne |date=2016-08-26 |website=WHATWG |access-date=2016-08-26 |url-status=live |archive-url=https://web.archive.org/web/20160826132911/https://fetch.spec.whatwg.org/#x-content-type-options-header |archive-date=2016-08-26}}`{=mediawiki}

[^44]: `{{cite web|url=https://stackoverflow.com/questions/1288338/why-does-asp-net-framework-add-the-x-powered-byasp-net-http-header-in-response |title=Why does ASP.NET framework add the 'X-Powered-By:ASP.NET' HTTP Header in responses? - Stack Overflow |accessdate=2010-09-30}}`{=mediawiki}

[^45]: 

[^46]: `{{cite web|url=http://msdn.microsoft.com/en-us/library/ie/cc288325%28v=vs.85%29.aspx#SetMode |title=Defining Document Compatibility: Specifying Document Compatibility Modes |date=2011-04-01 |accessdate=2012-01-24 }}`{=mediawiki}

[^47]: `{{cite web|url=http://blogs.msdn.com/b/ie/archive/2008/07/02/ie8-security-part-iv-the-xss-filter.aspx |title=IE8 Security Part IV: The XSS Filter |author=Eric Lawrence |date=2008-07-02 |accessdate=2010-09-30}}`{=mediawiki}

[^48]: `{{cite web|url=http://www.w3.org/TR/CSP/|title=Content Security Policy |publisher=W3C |year=2012|accessdate=28 April 2017}}`{=mediawiki}

[^49]: `{{cite web|url=http://tools.ietf.org/html/rfc7230#section-3.1.2|title=Hypertext Transfer Protocol (HTTP/1.1): Message Syntax and Routing|accessdate=2014-07-24}}`{=mediawiki}

[^50]: `{{Cite web|url=https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Timing-Allow-Origin|title=Timing-Allow-Origin|website=Mozilla Developer Network|language=en-US|access-date=2018-01-25}}`{=mediawiki}

[^51]: `{{cite web|url=https://developer.mozilla.org/en-US/docs/Web/HTTP/Configuring_servers_for_Ogg_media#Serve_X-Content-Duration_headers |title=Configuring servers for Ogg media |date=2014-05-26 |accessdate=2015-01-03}}`{=mediawiki}

[^52]: `{{cite web|url=http://blogs.msdn.com/b/ie/archive/2008/09/02/ie8-security-part-vi-beta-2-update.aspx |title=IE8 Security Part VI: Beta 2 Update |author=Eric Lawrence |date=2008-09-03 |accessdate=2010-09-28}}`{=mediawiki}

[^53]: `{{cite web|url=https://code.google.com/chrome/extensions/hosting.html |title=Hosting - Google Chrome Extensions - Google Code |accessdate=2012-06-14}}`{=mediawiki}

[^54]: `{{cite web |url=https://fetch.spec.whatwg.org/#x-content-type-options-header |title=Fetch standard |last1=van Kesteren |first1=Anne |date=2016-08-26 |website=WHATWG |access-date=2016-08-26 |url-status=live |archive-url=https://web.archive.org/web/20160826132911/https://fetch.spec.whatwg.org/#x-content-type-options-header |archive-date=2016-08-26}}`{=mediawiki}

[^55]: `{{cite web|url=https://stackoverflow.com/questions/1288338/why-does-asp-net-framework-add-the-x-powered-byasp-net-http-header-in-response |title=Why does ASP.NET framework add the 'X-Powered-By:ASP.NET' HTTP Header in responses? - Stack Overflow |accessdate=2010-09-30}}`{=mediawiki}

[^56]: 

[^57]: `{{cite web|url=http://msdn.microsoft.com/en-us/library/ie/cc288325%28v=vs.85%29.aspx#SetMode |title=Defining Document Compatibility: Specifying Document Compatibility Modes |date=2011-04-01 |accessdate=2012-01-24 }}`{=mediawiki}

[^58]: `{{cite web|url=http://blogs.msdn.com/b/ie/archive/2008/07/02/ie8-security-part-iv-the-xss-filter.aspx |title=IE8 Security Part IV: The XSS Filter |author=Eric Lawrence |date=2008-07-02 |accessdate=2010-09-30}}`{=mediawiki}
