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
