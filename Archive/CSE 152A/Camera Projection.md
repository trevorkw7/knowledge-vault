---
annotation-target: https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf
---


>%%
>```annotation-json
>{"created":"2024-01-25T01:22:52.095Z","text":"contains camera properties","updated":"2024-01-25T01:22:52.095Z","document":{"title":"lec04_cameraprojection.pdf","link":[{"href":"urn:x-pdf:b3888a5760f86bc431ef144e190d8ecb"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf"}],"documentFingerprint":"b3888a5760f86bc431ef144e190d8ecb"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","selector":[{"type":"TextPositionSelector","start":5095,"end":5105},{"type":"TextQuoteSelector","exact":"intrinsics","prefix":"handrakerPerspective projection(","suffix":") (converts from 3D rays to poin"}]}]}
>```
>%%
>*%%PREFIX%%handrakerPerspective projection(%%HIGHLIGHT%% ==intrinsics== %%POSTFIX%%) (converts from 3D rays to poin*
>%%LINK%%[[#^0x24o5dib5na|show annotation]]
>%%COMMENT%%
>contains camera properties
>%%TAGS%%
>
^0x24o5dib5na


>%%
>```annotation-json
>{"created":"2024-01-25T01:24:06.275Z","text":"takes -dx, -dy, z and converts it to -dx/z -dy/z","updated":"2024-01-25T01:24:06.275Z","document":{"title":"lec04_cameraprojection.pdf","link":[{"href":"urn:x-pdf:b3888a5760f86bc431ef144e190d8ecb"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf"}],"documentFingerprint":"b3888a5760f86bc431ef144e190d8ecb"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","selector":[{"type":"TextPositionSelector","start":4965,"end":4975},{"type":"TextQuoteSelector","exact":"intrinsics","prefix":"ight sidePerspective projection(","suffix":") (converts from 3D rays to poin"}]}]}
>```
>%%
>*%%PREFIX%%ight sidePerspective projection(%%HIGHLIGHT%% ==intrinsics== %%POSTFIX%%) (converts from 3D rays to poin*
>%%LINK%%[[#^cmn90aleqjs|show annotation]]
>%%COMMENT%%
>takes -dx, -dy, z and converts it to -dx/z -dy/z
>%%TAGS%%
>
^cmn90aleqjs


>%%
>```annotation-json
>{"created":"2024-01-25T01:27:34.836Z","text":"We need to convert from meters to pixels ","updated":"2024-01-25T01:27:34.836Z","document":{"title":"lec04_cameraprojection.pdf","link":[{"href":"urn:x-pdf:b3888a5760f86bc431ef144e190d8ecb"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf"}],"documentFingerprint":"b3888a5760f86bc431ef144e190d8ecb"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","selector":[{"type":"TextPositionSelector","start":5202,"end":5229},{"type":"TextQuoteSelector","exact":"From retina plane to images","prefix":" 152A, WI24: Manmohan Chandraker","suffix":"Pixels, bottom-left coordinate s"}]}]}
>```
>%%
>*%%PREFIX%%152A, WI24: Manmohan Chandraker%%HIGHLIGHT%% ==From retina plane to images== %%POSTFIX%%Pixels, bottom-left coordinate s*
>%%LINK%%[[#^ahzess1879r|show annotation]]
>%%COMMENT%%
>We need to convert from meters to pixels 
>%%TAGS%%
>
^ahzess1879r


>%%
>```annotation-json
>{"created":"2024-01-25T01:28:39.353Z","text":"Where the principle axis hits the image plane","updated":"2024-01-25T01:28:39.353Z","document":{"title":"lec04_cameraprojection.pdf","link":[{"href":"urn:x-pdf:b3888a5760f86bc431ef144e190d8ecb"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf"}],"documentFingerprint":"b3888a5760f86bc431ef144e190d8ecb"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","selector":[{"type":"TextPositionSelector","start":5450,"end":5456},{"type":"TextQuoteSelector","exact":"cx, cy","prefix":"cal coordinate systemxyxcycC’’=[","suffix":"]Step 1: Move center of image pl"}]}]}
>```
>%%
>*%%PREFIX%%cal coordinate systemxyxcycC’’=[%%HIGHLIGHT%% ==cx, cy== %%POSTFIX%%]Step 1: Move center of image pl*
>%%LINK%%[[#^y45rpw8f8fj|show annotation]]
>%%COMMENT%%
>Where the principle axis hits the image plane
>%%TAGS%%
>
^y45rpw8f8fj


>%%
>```annotation-json
>{"created":"2024-01-25T01:30:56.134Z","text":"Depend on the size of the pixel we have","updated":"2024-01-25T01:30:56.134Z","document":{"title":"lec04_cameraprojection.pdf","link":[{"href":"urn:x-pdf:b3888a5760f86bc431ef144e190d8ecb"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf"}],"documentFingerprint":"b3888a5760f86bc431ef144e190d8ecb"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","selector":[{"type":"TextPositionSelector","start":5697,"end":5755},{"type":"TextQuoteSelector","exact":"𝑝𝑥 pixels per meter along x𝑝𝑦 pixels per meter along y","prefix":"ange units from meters to pixels","suffix":"ijkCSE 152A, WI24: Manmohan Chan"}]}]}
>```
>%%
>*%%PREFIX%%ange units from meters to pixels%%HIGHLIGHT%% ==𝑝𝑥 pixels per meter along x𝑝𝑦 pixels per meter along y== %%POSTFIX%%ijkCSE 152A, WI24: Manmohan Chan*
>%%LINK%%[[#^neja5ecmyri|show annotation]]
>%%COMMENT%%
>Depend on the size of the pixel we have
>%%TAGS%%
>
^neja5ecmyri


>%%
>```annotation-json
>{"created":"2024-01-25T01:44:10.881Z","text":"Because adding a lens means pinhole camera model might not perfectly apply as the lens might not focus the light perfectly on the center of the sensor ","updated":"2024-01-25T01:44:10.881Z","document":{"title":"lec04_cameraprojection.pdf","link":[{"href":"urn:x-pdf:b3888a5760f86bc431ef144e190d8ecb"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf"}],"documentFingerprint":"b3888a5760f86bc431ef144e190d8ecb"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","selector":[{"type":"TextPositionSelector","start":5457,"end":5491},{"type":"TextQuoteSelector","exact":"Step 1: Move center of image plane","prefix":"rdinate systemxyxcycC’’=[cx, cy]","suffix":"CSE 152A, WI24: Manmohan Chandra"}]}]}
>```
>%%
>*%%PREFIX%%rdinate systemxyxcycC’’=[cx, cy]%%HIGHLIGHT%% ==Step 1: Move center of image plane== %%POSTFIX%%CSE 152A, WI24: Manmohan Chandra*
>%%LINK%%[[#^7dsqh2r3qs3|show annotation]]
>%%COMMENT%%
>Because adding a lens means pinhole camera model might not perfectly apply as the lens might not focus the light perfectly on the center of the sensor 
>%%TAGS%%
>
^7dsqh2r3qs3


>%%
>```annotation-json
>{"created":"2024-01-25T01:49:22.982Z","text":"These are unit vectors since they only stand for the axis. u, v, c are also unit vectors","updated":"2024-01-25T01:49:22.982Z","document":{"title":"lec04_cameraprojection.pdf","link":[{"href":"urn:x-pdf:b3888a5760f86bc431ef144e190d8ecb"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf"}],"documentFingerprint":"b3888a5760f86bc431ef144e190d8ecb"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","selector":[{"type":"TextPositionSelector","start":7338,"end":7400},{"type":"TextQuoteSelector","exact":"x-axis points right, y-axis points up, z-axis points backwards","prefix":"er of projection at the origin, ","suffix":")0Step 1: Translate by -cCSE 152"}]}]}
>```
>%%
>*%%PREFIX%%er of projection at the origin,%%HIGHLIGHT%% ==x-axis points right, y-axis points up, z-axis points backwards== %%POSTFIX%%)0Step 1: Translate by -cCSE 152*
>%%LINK%%[[#^nzucc4gxkr|show annotation]]
>%%COMMENT%%
>These are unit vectors since they only stand for the axis. u, v, c are also unit vectors
>%%TAGS%%
>
^nzucc4gxkr


>%%
>```annotation-json
>{"created":"2024-01-25T01:51:04.262Z","text":"Translate center of camera to the origin of the world by c","updated":"2024-01-25T01:51:04.262Z","document":{"title":"lec04_cameraprojection.pdf","link":[{"href":"urn:x-pdf:b3888a5760f86bc431ef144e190d8ecb"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf"}],"documentFingerprint":"b3888a5760f86bc431ef144e190d8ecb"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","selector":[{"type":"TextPositionSelector","start":7410,"end":7425},{"type":"TextQuoteSelector","exact":"Translate by -c","prefix":"-axis points backwards)0Step 1: ","suffix":"CSE 152A, WI24: Manmohan Chandra"}]}]}
>```
>%%
>*%%PREFIX%%-axis points backwards)0Step 1:%%HIGHLIGHT%% ==Translate by -c== %%POSTFIX%%CSE 152A, WI24: Manmohan Chandra*
>%%LINK%%[[#^45cwu0lfqt3|show annotation]]
>%%COMMENT%%
>Translate center of camera to the origin of the world by c
>%%TAGS%%
>
^45cwu0lfqt3


>%%
>```annotation-json
>{"created":"2024-01-25T02:06:43.561Z","text":"rotation - axis align\nproject - 3d plane to image plane\nk intrinsicits - move cooridnate system to bottom left corner, convert to pixels\ntranslation - align camera coordinate with world coordinate","updated":"2024-01-25T02:06:43.561Z","document":{"title":"lec04_cameraprojection.pdf","link":[{"href":"urn:x-pdf:b3888a5760f86bc431ef144e190d8ecb"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf"}],"documentFingerprint":"b3888a5760f86bc431ef144e190d8ecb"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","selector":[{"type":"TextPositionSelector","start":8361,"end":8390},{"type":"TextQuoteSelector","exact":"translationrotationprojection","prefix":", 0)T(0, 0, 1)TProjection matrix","suffix":"intrinsicsDenote this by t.CSE 1"}]}]}
>```
>%%
>*%%PREFIX%%, 0)T(0, 0, 1)TProjection matrix%%HIGHLIGHT%% ==translationrotationprojection== %%POSTFIX%%intrinsicsDenote this by t.CSE 1*
>%%LINK%%[[#^z5wu36uirn|show annotation]]
>%%COMMENT%%
>rotation - axis align
>project - 3d plane to image plane
>k intrinsicits - move cooridnate system to bottom left corner, convert to pixels
>translation - align camera coordinate with world coordinate
>%%TAGS%%
>
^z5wu36uirn


>%%
>```annotation-json
>{"created":"2024-01-25T02:20:49.223Z","text":"Everything that we can do with points we can also do with lines by doing the cross product. In this case we can take 2 points and take the cross product which makes it a line. We can also take 2 lines find the cross product and that represents the point","updated":"2024-01-25T02:20:49.223Z","document":{"title":"lec04_cameraprojection.pdf","link":[{"href":"urn:x-pdf:b3888a5760f86bc431ef144e190d8ecb"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf"}],"documentFingerprint":"b3888a5760f86bc431ef144e190d8ecb"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec04_cameraprojection.pdf","selector":[{"type":"TextPositionSelector","start":11269,"end":11276},{"type":"TextQuoteSelector","exact":"duality","prefix":"ese two lines?• Do you notice a ","suffix":"?Homogeneous points and linesCSE"}]}]}
>```
>%%
>*%%PREFIX%%ese two lines?• Do you notice a%%HIGHLIGHT%% ==duality== %%POSTFIX%%?Homogeneous points and linesCSE*
>%%LINK%%[[#^y9hu948nz5|show annotation]]
>%%COMMENT%%
>Everything that we can do with points we can also do with lines by doing the cross product. In this case we can take 2 points and take the cross product which makes it a line. We can also take 2 lines find the cross product and that represents the point
>%%TAGS%%
>
^y9hu948nz5
