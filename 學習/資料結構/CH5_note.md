---
annotation-target: DataStructure_Lecture_05_stack&queue.pdf
---

>%%
>```annotation-json
>{"created":"2023-04-10T05:23:56.919Z","text":"利用top指向最新進入的值","updated":"2023-04-10T05:23:56.919Z","document":{"title":"Data Structure","link":[{"href":"urn:x-pdf:725d62cb49de1c4290812d8fa1ea1b6a"},{"href":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf"}],"documentFingerprint":"725d62cb49de1c4290812d8fa1ea1b6a"},"uri":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","target":[{"source":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","selector":[{"type":"TextPositionSelector","start":194,"end":197},{"type":"TextQuoteSelector","exact":"top","prefix":"CBACBADCBAEDCBAtoptoptoptop top ","suffix":"*Figure 3.1: Inserting and delet"}]}]}
>```
>%%
>*%%PREFIX%%CBACBADCBAEDCBAtoptoptoptop top%%HIGHLIGHT%% ==top== %%POSTFIX%%*Figure 3.1: Inserting and delet*
>%%LINK%%[[#^y1xsqe6n4vt|show annotation]]
>%%COMMENT%%
>利用top指向最新進入的值
>%%TAGS%%
>
^y1xsqe6n4vt


>%%
>```annotation-json
>{"created":"2023-04-10T05:29:03.544Z","text":"empty stack","updated":"2023-04-10T05:29:03.544Z","document":{"title":"Data Structure","link":[{"href":"urn:x-pdf:725d62cb49de1c4290812d8fa1ea1b6a"},{"href":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf"}],"documentFingerprint":"725d62cb49de1c4290812d8fa1ea1b6a"},"uri":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","target":[{"source":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","selector":[{"type":"TextPositionSelector","start":1285,"end":1297},{"type":"TextQuoteSelector","exact":"int top = -1","prefix":"t;element stack[MAX_STACK_SIZE];","suffix":";BooleanIsEmpty(Stack) ::= top< "}]}]}
>```
>%%
>*%%PREFIX%%t;element stack[MAX_STACK_SIZE];%%HIGHLIGHT%% ==int top = -1== %%POSTFIX%%;BooleanIsEmpty(Stack) ::= top<*
>%%LINK%%[[#^kswiv3fqhq|show annotation]]
>%%COMMENT%%
>empty stack
>%%TAGS%%
>
^kswiv3fqhq



>%%
>```annotation-json
>{"created":"2023-04-10T05:31:28.866Z","text":"有指定時\n++top:先加再指定\ntop++:先指定再加\n\n(top+1=item的話 top還是原值)","updated":"2023-04-10T05:31:28.866Z","document":{"title":"Data Structure","link":[{"href":"urn:x-pdf:725d62cb49de1c4290812d8fa1ea1b6a"},{"href":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf"}],"documentFingerprint":"725d62cb49de1c4290812d8fa1ea1b6a"},"uri":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","target":[{"source":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","selector":[{"type":"TextPositionSelector","start":1504,"end":1524},{"type":"TextQuoteSelector","exact":"stack[++*top] = item","prefix":"SIZE-1)  {stack_full( );return;}","suffix":";}*program 3.1: Add to a stack ("}]}]}
>```
>%%
>*%%PREFIX%%SIZE-1)  {stack_full( );return;}%%HIGHLIGHT%% ==stack[++*top] = item== %%POSTFIX%%;}*program 3.1: Add to a stack (*
>%%LINK%%[[#^25filte5t|show annotation]]
>%%COMMENT%%
>有指定時
>++top:先加再指定
>top++:先指定再加
>
>(top+1=item的話 top還是原值)
>%%TAGS%%
>
^25filte5t


>%%
>```annotation-json
>{"created":"2023-04-10T05:36:12.718Z","text":"指向第一筆的前一筆","updated":"2023-04-10T05:36:12.718Z","document":{"title":"Data Structure","link":[{"href":"urn:x-pdf:725d62cb49de1c4290812d8fa1ea1b6a"},{"href":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf"}],"documentFingerprint":"725d62cb49de1c4290812d8fa1ea1b6a"},"uri":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","target":[{"source":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","selector":[{"type":"TextPositionSelector","start":1949,"end":1954},{"type":"TextQuoteSelector","exact":"front","prefix":"OUT (FIFO) LISTABACBADCBADCBrear","suffix":"rearfrontrearfrontrearfrontrearf"}]}]}
>```
>%%
>*%%PREFIX%%OUT (FIFO) LISTABACBADCBADCBrear%%HIGHLIGHT%% ==front== %%POSTFIX%%rearfrontrearfrontrearfrontrearf*
>%%LINK%%[[#^snsygqw9nrn|show annotation]]
>%%COMMENT%%
>指向第一筆的前一筆
>%%TAGS%%
>
^snsygqw9nrn


>%%
>```annotation-json
>{"created":"2023-04-10T05:49:44.291Z","text":"不然rare 會跑掉\n會超過maxqueuesize\n\n-----------\n環狀\ndetect front==rare?\n會有一個空位存在\n不然無法分辨滿與空(front=rare)","updated":"2023-04-10T05:49:44.291Z","document":{"title":"Data Structure","link":[{"href":"urn:x-pdf:725d62cb49de1c4290812d8fa1ea1b6a"},{"href":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf"}],"documentFingerprint":"725d62cb49de1c4290812d8fa1ea1b6a"},"uri":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","target":[{"source":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","selector":[{"type":"TextPositionSelector","start":3411,"end":3417},{"type":"TextQuoteSelector","exact":"SIZE-1","prefix":"lQ(queue) ::= rear == MAX_QUEUE_","suffix":"IMPLEMENTATION 1: USING ARRAYvoi"}]}]}
>```
>%%
>*%%PREFIX%%lQ(queue) ::= rear == MAX_QUEUE_%%HIGHLIGHT%% ==SIZE-1== %%POSTFIX%%IMPLEMENTATION 1: USING ARRAYvoi*
>%%LINK%%[[#^kmmnt2cuyg|show annotation]]
>%%COMMENT%%
>不然rare 會跑掉
>會超過maxqueuesize
>
>-----------
>環狀
>detect front==rare?
>會有一個空位存在
>不然無法分辨滿與空(front=rare)
>%%TAGS%%
>
^kmmnt2cuyg


>%%
>```annotation-json
>{"created":"2023-04-10T06:01:57.660Z","text":"改成enqueue 會更好","updated":"2023-04-10T06:01:57.660Z","document":{"title":"Data Structure","link":[{"href":"urn:x-pdf:725d62cb49de1c4290812d8fa1ea1b6a"},{"href":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf"}],"documentFingerprint":"725d62cb49de1c4290812d8fa1ea1b6a"},"uri":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","target":[{"source":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","selector":[{"type":"TextPositionSelector","start":5526,"end":5530},{"type":"TextQuoteSelector","exact":"addq","prefix":" is left when queue is fullvoid ","suffix":"(int front, int *rear, element i"}]}]}
>```
>%%
>*%%PREFIX%%is left when queue is fullvoid%%HIGHLIGHT%% ==addq== %%POSTFIX%%(int front, int *rear, element i*
>%%LINK%%[[#^wvcsvmfa4ya|show annotation]]
>%%COMMENT%%
>改成enqueue 會更好
>%%TAGS%%
>
^wvcsvmfa4ya


>%%
>```annotation-json
>{"created":"2023-04-10T06:09:52.057Z","updated":"2023-04-10T06:09:52.057Z","document":{"title":"Data Structure","link":[{"href":"urn:x-pdf:725d62cb49de1c4290812d8fa1ea1b6a"},{"href":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf"}],"documentFingerprint":"725d62cb49de1c4290812d8fa1ea1b6a"},"uri":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","target":[{"source":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","selector":[{"type":"TextPositionSelector","start":9557,"end":9582},{"type":"TextQuoteSelector","exact":"EVALUATION OF EXPRESSIONS","prefix":"ecedence rule + associative rule","suffix":"• Infix:• Each operator comes in"}]}]}
>```
>%%
>*%%PREFIX%%ecedence rule + associative rule%%HIGHLIGHT%% ==EVALUATION OF EXPRESSIONS== %%POSTFIX%%• Infix:• Each operator comes in*
>%%LINK%%[[#^gken1hzstmv|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#考點
^gken1hzstmv


>%%
>```annotation-json
>{"created":"2023-04-10T06:25:24.445Z","updated":"2023-04-10T06:25:24.445Z","document":{"title":"Data Structure","link":[{"href":"urn:x-pdf:725d62cb49de1c4290812d8fa1ea1b6a"},{"href":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf"}],"documentFingerprint":"725d62cb49de1c4290812d8fa1ea1b6a"},"uri":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","target":[{"source":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","selector":[{"type":"TextPositionSelector","start":9821,"end":9858},{"type":"TextQuoteSelector","exact":" Phase 1: Infix to postfix conversion","prefix":"LUATION OF EXPRESSIONS (CONT’D)•","suffix":"• 6/2-3+4*2 → 6 2 / 3 – 4 2 * +•"}]}]}
>```
>%%
>*%%PREFIX%%LUATION OF EXPRESSIONS (CONT’D)•%%HIGHLIGHT%% ==Phase 1: Infix to postfix conversion== %%POSTFIX%%• 6/2-3+4*2 → 6 2 / 3 – 4 2 * +•*
>%%LINK%%[[#^ac4mfh0jwb|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#考點
^ac4mfh0jwb


>%%
>```annotation-json
>{"created":"2023-04-10T06:24:18.633Z","text":"最後一個\n由左到右加上括號","updated":"2023-04-10T06:24:18.633Z","document":{"title":"Data Structure","link":[{"href":"urn:x-pdf:725d62cb49de1c4290812d8fa1ea1b6a"},{"href":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf"}],"documentFingerprint":"725d62cb49de1c4290812d8fa1ea1b6a"},"uri":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","target":[{"source":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","selector":[{"type":"TextPositionSelector","start":9818,"end":9819},{"type":"TextQuoteSelector","exact":"D","prefix":"EVALUATION OF EXPRESSIONS (CONT’","suffix":")• Phase 1: Infix to postfix con"}]}]}
>```
>%%
>*%%PREFIX%%EVALUATION OF EXPRESSIONS (CONT’%%HIGHLIGHT%% ==D== %%POSTFIX%%)• Phase 1: Infix to postfix con*
>%%LINK%%[[#^2nomacsxq7f|show annotation]]
>%%COMMENT%%
>最後一個
>由左到右加上括號
>%%TAGS%%
>
^2nomacsxq7f


>%%
>```annotation-json
>{"created":"2023-04-10T06:33:47.613Z","text":"![image.png](https://raw.githubusercontent.com/laudantstolam/imagesource/main/ds_transform.png)\n","updated":"2023-04-10T06:33:47.613Z","document":{"title":"Data Structure","link":[{"href":"urn:x-pdf:725d62cb49de1c4290812d8fa1ea1b6a"},{"href":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf"}],"documentFingerprint":"725d62cb49de1c4290812d8fa1ea1b6a"},"uri":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","target":[{"source":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","selector":[{"type":"TextPositionSelector","start":10060,"end":10069},{"type":"TextQuoteSelector","exact":"23-5*93/+","prefix":"N EVALUATIONPOSTFIX EVALUATION• ","suffix":"38GOAL: INFIX --> POSTFIX#define"}]}]}
>```
>%%
>*%%PREFIX%%N EVALUATIONPOSTFIX EVALUATION•%%HIGHLIGHT%% ==23-5*93/+== %%POSTFIX%%38GOAL: INFIX --> POSTFIX#define*
>%%LINK%%[[#^t2fm0ugv4q|show annotation]]
>%%COMMENT%%
>![image.png](https://raw.githubusercontent.com/laudantstolam/imagesource/main/ds_transform.png)
>
>%%TAGS%%
>
^t2fm0ugv4q


>%%
>```annotation-json
>{"created":"2023-04-17T05:31:47.871Z","text":"1.=-+a*bc/de\n3.=^^ABC","updated":"2023-04-17T05:31:47.871Z","document":{"title":"Data Structure","link":[{"href":"urn:x-pdf:725d62cb49de1c4290812d8fa1ea1b6a"},{"href":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf"}],"documentFingerprint":"725d62cb49de1c4290812d8fa1ea1b6a"},"uri":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","target":[{"source":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","selector":[{"type":"TextPositionSelector","start":13395,"end":13408},{"type":"TextQuoteSelector","exact":"Infix →Prefix","prefix":"NT) INFIX TO PREFIX CONVERSION• ","suffix":"(1) a+b*c-d/e(2) (a+b)*(c-d)/(e*"}]}]}
>```
>%%
>*%%PREFIX%%NT) INFIX TO PREFIX CONVERSION•%%HIGHLIGHT%% ==Infix →Prefix== %%POSTFIX%%(1) a+b*c-d/e(2) (a+b)*(c-d)/(e**
>%%LINK%%[[#^pxjq15fq63b|show annotation]]
>%%COMMENT%%
>1.=-+a*bc/de
>3.=^^ABC
>%%TAGS%%
>
^pxjq15fq63b


>%%
>```annotation-json
>{"created":"2023-04-17T05:40:29.478Z","text":"``\n2.\n=a*(b+(c*d))/e-f\n=a*(b+c*d)/e-f\n``","updated":"2023-04-17T05:40:29.478Z","document":{"title":"Data Structure","link":[{"href":"urn:x-pdf:725d62cb49de1c4290812d8fa1ea1b6a"},{"href":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf"}],"documentFingerprint":"725d62cb49de1c4290812d8fa1ea1b6a"},"uri":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","target":[{"source":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","selector":[{"type":"TextPositionSelector","start":13486,"end":13499},{"type":"TextQuoteSelector","exact":"Prefix →Infix","prefix":"4) ~(A>B) and (C or D<E) or ~F• ","suffix":"(1) +*/ab-+cde-fg(2) -/*a+b*cdef"}]}]}
>```
>%%
>*%%PREFIX%%4) ~(A>B) and (C or D<E) or ~F•%%HIGHLIGHT%% ==Prefix →Infix== %%POSTFIX%%(1) +*/ab-+cde-fg(2) -/*a+b*cdef*
>%%LINK%%[[#^kw4tylue9m|show annotation]]
>%%COMMENT%%
>``
>2.
>=a*(b+(c*d))/e-f
>=a*(b+c*d)/e-f
>``
>%%TAGS%%
>
^kw4tylue9m


>%%
>```annotation-json
>{"created":"2023-04-17T05:46:28.457Z","text":"1. abc*+de/-\n或是abc*de/-+>>先減再加\n2.ab+cd-*ef*g^\n4.=(~(A<B)and(C and D<E)or ~F)\n=AB>~CDE<or and F~ or","updated":"2023-04-17T05:46:28.457Z","document":{"title":"Data Structure","link":[{"href":"urn:x-pdf:725d62cb49de1c4290812d8fa1ea1b6a"},{"href":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf"}],"documentFingerprint":"725d62cb49de1c4290812d8fa1ea1b6a"},"uri":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","target":[{"source":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","selector":[{"type":"TextPositionSelector","start":12913,"end":12927},{"type":"TextQuoteSelector","exact":"Infix →Postfix","prefix":"t unstackedRULESRULES (CONT’D)• ","suffix":"(1) a+b*c-d/e(2) (a+b)*(c-d)/(e*"}]}]}
>```
>%%
>*%%PREFIX%%t unstackedRULESRULES (CONT’D)•%%HIGHLIGHT%% ==Infix →Postfix== %%POSTFIX%%(1) a+b*c-d/e(2) (a+b)*(c-d)/(e**
>%%LINK%%[[#^dslp2w6ywqk|show annotation]]
>%%COMMENT%%
>1. abc*+de/-
>或是abc*de/-+>>先減再加
>2.ab+cd-*ef*g^
>4.=(~(A<B)and(C and D<E)or ~F)
>=AB>~CDE<or and F~ or
>%%TAGS%%
>
^dslp2w6ywqk


>%%
>```annotation-json
>{"created":"2023-04-17T05:47:52.438Z","text":"1.\na/(b-c+d)*(e-a)*c","updated":"2023-04-17T05:47:52.438Z","document":{"title":"Data Structure","link":[{"href":"urn:x-pdf:725d62cb49de1c4290812d8fa1ea1b6a"},{"href":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf"}],"documentFingerprint":"725d62cb49de1c4290812d8fa1ea1b6a"},"uri":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","target":[{"source":"vault:/%E5%AD%B8%E7%BF%92/%E8%B3%87%E6%96%99%E7%B5%90%E6%A7%8B/DataStructure_Lecture_05_stack&queue.pdf","selector":[{"type":"TextPositionSelector","start":13005,"end":13019},{"type":"TextQuoteSelector","exact":"Postfix →Infix","prefix":"4) ~(A>B) and (C or D<E) or ~F• ","suffix":"(1) abc-d+/ea-*c*(2) ABCDE-+^*EF"}]}]}
>```
>%%
>*%%PREFIX%%4) ~(A>B) and (C or D<E) or ~F•%%HIGHLIGHT%% ==Postfix →Infix== %%POSTFIX%%(1) abc-d+/ea-*c*(2) ABCDE-+^*EF*
>%%LINK%%[[#^6avmtvh46g3|show annotation]]
>%%COMMENT%%
>1.
>a/(b-c+d)*(e-a)*c
>%%TAGS%%
>
^6avmtvh46g3
