---
annotation-target: https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf
---


>%%
>```annotation-json
>{"created":"2024-02-03T01:36:24.157Z","text":"Image has moved a bit but the intensity should be about the same around matching points","updated":"2024-02-03T01:36:24.157Z","document":{"title":"lec07_matching.pdf","link":[{"href":"urn:x-pdf:69d00295bab0306dc8262d699d6f27a8"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf"}],"documentFingerprint":"69d00295bab0306dc8262d699d6f27a8"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf","selector":[{"type":"TextPositionSelector","start":5154,"end":5180},{"type":"TextQuoteSelector","exact":"Sum of Squared Differences","prefix":"erSimple matching methods• SSD (","suffix":")W1(x, y): k x k pixel patch in "}]}]}
>```
>%%
>*%%PREFIX%%erSimple matching methods• SSD (%%HIGHLIGHT%% ==Sum of Squared Differences== %%POSTFIX%%)W1(x, y): k x k pixel patch in*
>%%LINK%%[[#^c77s19prtwb|show annotation]]
>%%COMMENT%%
>Image has moved a bit but the intensity should be about the same around matching points
>%%TAGS%%
>
^c77s19prtwb


>%%
>```annotation-json
>{"created":"2024-02-03T01:37:56.132Z","text":"For a given patch in the first image, we test all other patches in the second image and choose whichever patch has the smallest difference.","updated":"2024-02-03T01:37:56.132Z","document":{"title":"lec07_matching.pdf","link":[{"href":"urn:x-pdf:69d00295bab0306dc8262d699d6f27a8"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf"}],"documentFingerprint":"69d00295bab0306dc8262d699d6f27a8"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf","selector":[{"type":"TextPositionSelector","start":5317,"end":5348},{"type":"TextQuoteSelector","exact":"SSD (Sum of Squared Differences","prefix":"ndrakerSimple matching methods• ","suffix":")• NCC (Normalized Cross Correla"}]}]}
>```
>%%
>*%%PREFIX%%ndrakerSimple matching methods•%%HIGHLIGHT%% ==SSD (Sum of Squared Differences== %%POSTFIX%%)• NCC (Normalized Cross Correla*
>%%LINK%%[[#^jjcpro0hzua|show annotation]]
>%%COMMENT%%
>For a given patch in the first image, we test all other patches in the second image and choose whichever patch has the smallest difference.
>%%TAGS%%
>
^jjcpro0hzua


>%%
>```annotation-json
>{"created":"2024-02-03T01:39:32.576Z","text":"More resistant to uniform illumination changes","updated":"2024-02-03T01:39:32.576Z","document":{"title":"lec07_matching.pdf","link":[{"href":"urn:x-pdf:69d00295bab0306dc8262d699d6f27a8"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf"}],"documentFingerprint":"69d00295bab0306dc8262d699d6f27a8"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf","selector":[{"type":"TextPositionSelector","start":5409,"end":5412},{"type":"TextQuoteSelector","exact":"NCC","prefix":"elation)• What advantages might ","suffix":" have over SSD?,(Mean) (Standard"}]}]}
>```
>%%
>*%%PREFIX%%elation)• What advantages might%%HIGHLIGHT%% ==NCC== %%POSTFIX%%have over SSD?,(Mean) (Standard*
>%%LINK%%[[#^kcf3lva9k5|show annotation]]
>%%COMMENT%%
>More resistant to uniform illumination changes
>%%TAGS%%
>
^kcf3lva9k5


>%%
>```annotation-json
>{"created":"2024-02-03T01:43:26.304Z","text":"SSD for example","updated":"2024-02-03T01:43:26.304Z","document":{"title":"lec07_matching.pdf","link":[{"href":"urn:x-pdf:69d00295bab0306dc8262d699d6f27a8"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf"}],"documentFingerprint":"69d00295bab0306dc8262d699d6f27a8"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf","selector":[{"type":"TextPositionSelector","start":5648,"end":5665},{"type":"TextQuoteSelector","exact":"distance function","prefix":" the best match in I2?1. Define ","suffix":" that compares two descriptors2."}]}]}
>```
>%%
>*%%PREFIX%%the best match in I2?1. Define%%HIGHLIGHT%% ==distance function== %%POSTFIX%%that compares two descriptors2.*
>%%LINK%%[[#^0iq1ug0trruw|show annotation]]
>%%COMMENT%%
>SSD for example
>%%TAGS%%
>
^0iq1ug0trruw


>%%
>```annotation-json
>{"created":"2024-02-03T01:49:42.923Z","text":"ratio will start approaching 1 as feature becomes more ambiguos","updated":"2024-02-03T01:49:42.923Z","document":{"title":"lec07_matching.pdf","link":[{"href":"urn:x-pdf:69d00295bab0306dc8262d699d6f27a8"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf"}],"documentFingerprint":"69d00295bab0306dc8262d699d6f27a8"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf","selector":[{"type":"TextPositionSelector","start":6623,"end":6649},{"type":"TextQuoteSelector","exact":"SSD(f1, f2) / SSD(f1, f2’)","prefix":"ter approach:  ratio distance = ","suffix":"– f2 is best SSD match to f1 in "}]}]}
>```
>%%
>*%%PREFIX%%ter approach:  ratio distance =%%HIGHLIGHT%% ==SSD(f1, f2) / SSD(f1, f2’)== %%POSTFIX%%– f2 is best SSD match to f1 in*
>%%LINK%%[[#^z12kpnygg0j|show annotation]]
>%%COMMENT%%
>ratio will start approaching 1 as feature becomes more ambiguos
>%%TAGS%%
>
^z12kpnygg0j



>%%
>```annotation-json
>{"created":"2024-02-03T01:55:01.400Z","text":"maxizmize true positives and minimize false positives, to maximize true positives we need to increase threshold and to minimize false positives we need to decrease threshold. we must comprimise because these are opposing","updated":"2024-02-03T01:55:01.400Z","document":{"title":"lec07_matching.pdf","link":[{"href":"urn:x-pdf:69d00295bab0306dc8262d699d6f27a8"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf"}],"documentFingerprint":"69d00295bab0306dc8262d699d6f27a8"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf","selector":[{"type":"TextPositionSelector","start":7462,"end":7473},{"type":"TextQuoteSelector","exact":"performance","prefix":"sThe distance threshold affects ","suffix":"• True positives = number of det"}]}]}
>```
>%%
>*%%PREFIX%%sThe distance threshold affects%%HIGHLIGHT%% ==performance== %%POSTFIX%%• True positives = number of det*
>%%LINK%%[[#^ocajs4ss7rq|show annotation]]
>%%COMMENT%%
>maxizmize true positives and minimize false positives, to maximize true positives we need to increase threshold and to minimize false positives we need to decrease threshold. we must comprimise because these are opposing
>%%TAGS%%
>
^ocajs4ss7rq


>%%
>```annotation-json
>{"created":"2024-02-03T02:14:31.277Z","text":"If the disparity is smaller, the object is farther away. We can compute depth using this idea","updated":"2024-02-03T02:14:31.277Z","document":{"title":"lec07_matching.pdf","link":[{"href":"urn:x-pdf:69d00295bab0306dc8262d699d6f27a8"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf"}],"documentFingerprint":"69d00295bab0306dc8262d699d6f27a8"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec07_matching.pdf","selector":[{"type":"TextPositionSelector","start":9533,"end":9577},{"type":"TextQuoteSelector","exact":"Depth is inversely proportional to disparity","prefix":" X0−dZ0 Using similar triangles:","suffix":"Z0X0 - dfCSE 152A, WI24: Manmoha"}]}]}
>```
>%%
>*%%PREFIX%%X0−dZ0 Using similar triangles:%%HIGHLIGHT%% ==Depth is inversely proportional to disparity== %%POSTFIX%%Z0X0 - dfCSE 152A, WI24: Manmoha*
>%%LINK%%[[#^mtao6j2dfvl|show annotation]]
>%%COMMENT%%
>If the disparity is smaller, the object is farther away. We can compute depth using this idea
>%%TAGS%%
>
^mtao6j2dfvl
