---
annotation-target: https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf
---


>%%
>```annotation-json
>{"created":"2024-02-10T01:13:27.914Z","updated":"2024-02-10T01:13:27.914Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":3631,"end":3653},{"type":"TextQuoteSelector","exact":"Harris Corner Detector","prefix":"s often used in practice𝑲𝑥𝑲𝑦","suffix":"CSE 152A, WI24: Manmohan Chandra"}]}]}
>```
>%%
>*%%PREFIX%%s often used in practice𝑲𝑥𝑲𝑦%%HIGHLIGHT%% ==Harris Corner Detector== %%POSTFIX%%CSE 152A, WI24: Manmohan Chandra*
>%%LINK%%[[#^ddf2d4ki2km|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^ddf2d4ki2km


>%%
>```annotation-json
>{"created":"2024-02-10T01:17:10.179Z","text":"Given a point p in image 1, point q in image 2 is constrained to be on a straight line. This is because the 3d point lies somewhere on the back projected ray r. This is a line in 3d space. Points project to points, lines project to lines. Therefore the projection onto image 2 must be a line.","updated":"2024-02-10T01:17:10.179Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":4807,"end":4820},{"type":"TextQuoteSelector","exact":"epipolar line","prefix":"the epipolar line.epipolar plane","suffix":"epipolar line03D point lies some"}]}]}
>```
>%%
>*%%PREFIX%%the epipolar line.epipolar plane%%HIGHLIGHT%% ==epipolar line== %%POSTFIX%%epipolar line03D point lies some*
>%%LINK%%[[#^zvuu85cdine|show annotation]]
>%%COMMENT%%
>Given a point p in image 1, point q in image 2 is constrained to be on a straight line. This is because the 3d point lies somewhere on the back projected ray r. This is a line in 3d space. Points project to points, lines project to lines. Therefore the projection onto image 2 must be a line.
>%%TAGS%%
>
^zvuu85cdine


>%%
>```annotation-json
>{"created":"2024-02-10T01:22:18.765Z","updated":"2024-02-10T01:22:18.765Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":5264,"end":5270},{"type":"TextQuoteSelector","exact":"      ","prefix":"xel space:                      ","suffix":"               . • Rearranging:•"}]}]}
>```
>%%
>*%%PREFIX%%xel space:%%HIGHLIGHT%% ==== %%POSTFIX%%. • Rearranging:•*
>%%LINK%%[[#^7enarkf5vib|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^7enarkf5vib


>%%
>```annotation-json
>{"created":"2024-02-10T01:22:22.946Z","text":"K1 is intrinsic paramter matrix for p and K2 is for q. We can define q' p' which are in pixel coordinates. We define F as a 3x3 matrix with 7 degrees of freedom. F is rank 2 because E is rank 2 since E = [t]x R. F is rank 2. 7 Degrees of freedom for F","updated":"2024-02-10T01:22:22.946Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":5242,"end":5285},{"type":"TextQuoteSelector","exact":"                                           ","prefix":"atrix constraint in pixel space:","suffix":". • Rearranging:• Define:• Then,"}]}]}
>```
>%%
>*%%PREFIX%%atrix constraint in pixel space:%%HIGHLIGHT%% ==== %%POSTFIX%%. • Rearranging:• Define:• Then,*
>%%LINK%%[[#^mz3s8fr2ddh|show annotation]]
>%%COMMENT%%
>K1 is intrinsic paramter matrix for p and K2 is for q. We can define q' p' which are in pixel coordinates. We define F as a 3x3 matrix with 7 degrees of freedom. F is rank 2 because E is rank 2 since E = [t]x R. F is rank 2. 7 Degrees of freedom for F
>%%TAGS%%
>
^mz3s8fr2ddh


>%%
>```annotation-json
>{"created":"2024-02-10T01:19:53.059Z","text":"This is a 3 X 3 matrix that satisfies qTEp = 0. 5 Degrees of freedom. Rotation matrix has 3 degrees of freedom R. t is a 3d vector so 3 degrees of freedom for t. We lose 1 degree of freedom for scale since E is a homogenous entity. This means that we can arbitrarily scale E and the result will still be 0/.","updated":"2024-02-10T01:19:53.059Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":4968,"end":4984},{"type":"TextQuoteSelector","exact":"Essential matrix","prefix":" have: • Define:• Then, we have:","suffix":"Essential matrixHow many degrees"}]}]}
>```
>%%
>*%%PREFIX%%have: • Define:• Then, we have:%%HIGHLIGHT%% ==Essential matrix== %%POSTFIX%%Essential matrixHow many degrees*
>%%LINK%%[[#^gd45u97m0oo|show annotation]]
>%%COMMENT%%
>This is a 3 X 3 matrix that satisfies qTEp = 0. 5 Degrees of freedom. Rotation matrix has 3 degrees of freedom R. t is a 3d vector so 3 degrees of freedom for t. We lose 1 degree of freedom for scale since E is a homogenous entity. This means that we can arbitrarily scale E and the result will still be 0/.
>%%TAGS%%
>
^gd45u97m0oo


>%%
>```annotation-json
>{"created":"2024-02-10T01:26:05.909Z","text":"We derived F from the intrinsic parameter matricies but we don't actually need this because we can estimate F given enough corrispondences.","updated":"2024-02-10T01:26:05.909Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":5974,"end":5976},{"type":"TextQuoteSelector","exact":" F","prefix":"4: Manmohan ChandrakerEstimating","suffix":"•Given just the two images, can "}]}]}
>```
>%%
>*%%PREFIX%%4: Manmohan ChandrakerEstimating%%HIGHLIGHT%% ==F== %%POSTFIX%%•Given just the two images, can*
>%%LINK%%[[#^wqyc71em8ol|show annotation]]
>%%COMMENT%%
>We derived F from the intrinsic parameter matricies but we don't actually need this because we can estimate F given enough corrispondences.
>%%TAGS%%
>
^wqyc71em8ol


>%%
>```annotation-json
>{"created":"2024-02-10T01:27:38.776Z","text":"Homogenous coordinates for each point in each image.","updated":"2024-02-10T01:27:38.776Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":6231,"end":6263},{"type":"TextQuoteSelector","exact":" x = (u,v,1)T and x’ = (u’,v’,1)","prefix":"hes x and x’ in two images.• Let","suffix":"T,•Each match gives a linear equ"}]}]}
>```
>%%
>*%%PREFIX%%hes x and x’ in two images.• Let%%HIGHLIGHT%% ==x = (u,v,1)T and x’ = (u’,v’,1)== %%POSTFIX%%T,•Each match gives a linear equ*
>%%LINK%%[[#^16qtdzrh8k|show annotation]]
>%%COMMENT%%
>Homogenous coordinates for each point in each image.
>%%TAGS%%
>
^16qtdzrh8k


>%%
>```annotation-json
>{"created":"2024-02-10T01:28:44.205Z","text":"Expansion will result in a 1X1 scalar that should equal to 0. 9 unknowns and u and v (pixel coordinates).","updated":"2024-02-10T01:28:44.205Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":6266,"end":6300},{"type":"TextQuoteSelector","exact":"Each match gives a linear equation","prefix":"= (u,v,1)T and x’ = (u’,v’,1)T,•","suffix":":0''''''333231232221131211=+++++"}]}]}
>```
>%%
>*%%PREFIX%%= (u,v,1)T and x’ = (u’,v’,1)T,•%%HIGHLIGHT%% ==Each match gives a linear equation== %%POSTFIX%%:0''''''333231232221131211=+++++*
>%%LINK%%[[#^8i9zjmmd24y|show annotation]]
>%%COMMENT%%
>Expansion will result in a 1X1 scalar that should equal to 0. 9 unknowns and u and v (pixel coordinates).
>%%TAGS%%
>
^8i9zjmmd24y


>%%
>```annotation-json
>{"created":"2024-02-10T01:32:10.171Z","text":"Each row here in A is made up of coefficients for the fs to solve the = 0 linear equation. A is a n x 9 matrix. This is not a normal system of equations because Ax = 0. A must be a 8x9 matrix since x is a 9x1 vector. ","updated":"2024-02-10T01:32:10.171Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":6772,"end":6791},{"type":"TextQuoteSelector","exact":"system of equations","prefix":"point correspondences, set up a ","suffix":":CSE 152A, WI24: Manmohan Chandr"}]}]}
>```
>%%
>*%%PREFIX%%point correspondences, set up a%%HIGHLIGHT%% ==system of equations== %%POSTFIX%%:CSE 152A, WI24: Manmohan Chandr*
>%%LINK%%[[#^ifoggtc56t|show annotation]]
>%%COMMENT%%
>Each row here in A is made up of coefficients for the fs to solve the = 0 linear equation. A is a n x 9 matrix. This is not a normal system of equations because Ax = 0. A must be a 8x9 matrix since x is a 9x1 vector. 
>%%TAGS%%
>
^ifoggtc56t


>%%
>```annotation-json
>{"created":"2024-02-10T01:37:59.755Z","text":"Because we have a trivial sollution where f = 0.","updated":"2024-02-10T01:37:59.755Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":6695,"end":6724},{"type":"TextQuoteSelector","exact":"we seek f to minimize        ","prefix":"instead of solving            , ","suffix":" .0=AfAfGiven n point correspond"}]}]}
>```
>%%
>*%%PREFIX%%instead of solving            ,%%HIGHLIGHT%% ==we seek f to minimize== %%POSTFIX%%.0=AfAfGiven n point correspond*
>%%LINK%%[[#^tyt7s0fhfi|show annotation]]
>%%COMMENT%%
>Because we have a trivial sollution where f = 0.
>%%TAGS%%
>
^tyt7s0fhfi


>%%
>```annotation-json
>{"created":"2024-02-10T01:42:09.314Z","text":"s1 ... sn are the singular values of n, always in decending order from s1 (largest) to sn (smallest). column of v is the solution of this homogenous system.","updated":"2024-02-10T01:42:09.314Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":6933,"end":6960},{"type":"TextQuoteSelector","exact":"Singular value decompositio","prefix":"e seek f to minimize          .•","suffix":"n:•Solution f given by the last "}]}]}
>```
>%%
>*%%PREFIX%%e seek f to minimize          .•%%HIGHLIGHT%% ==Singular value decompositio== %%POSTFIX%%n:•Solution f given by the last*
>%%LINK%%[[#^vpwpx0td6|show annotation]]
>%%COMMENT%%
>s1 ... sn are the singular values of n, always in decending order from s1 (largest) to sn (smallest). column of v is the solution of this homogenous system.
>%%TAGS%%
>
^vpwpx0td6


>%%
>```annotation-json
>{"created":"2024-02-10T01:47:12.075Z","text":"2 Independently linear columns","updated":"2024-02-10T01:47:12.075Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":7080,"end":7086},{"type":"TextQuoteSelector","exact":"rank 2","prefix":" Method: Problem?•F should have ","suffix":"•To enforce that F is of rank 2,"}]}]}
>```
>%%
>*%%PREFIX%%Method: Problem?•F should have%%HIGHLIGHT%% ==rank 2== %%POSTFIX%%•To enforce that F is of rank 2,*
>%%LINK%%[[#^qp11t3weg3|show annotation]]
>%%COMMENT%%
>2 Independently linear columns
>%%TAGS%%
>
^qp11t3weg3


>%%
>```annotation-json
>{"created":"2024-02-10T01:48:30.859Z","text":"Set sigma 3 to be 0 and multiply back with the two rotation matrix for F'. This is the closest matrix that is rank 2 matrix (in general n-k matrix).","updated":"2024-02-10T01:48:30.859Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":7375,"end":7376},{"type":"TextQuoteSelector","exact":"0","prefix":"ûùêêêëé=321000000Σsssúúúûùêêêëé=","suffix":"000000Σ'21ssT=VUFΣ''CSE 152A, WI"}]}]}
>```
>%%
>*%%PREFIX%%ûùêêêëé=321000000Σsssúúúûùêêêëé=%%HIGHLIGHT%% ==0== %%POSTFIX%%000000Σ'21ssT=VUFΣ''CSE 152A, WI*
>%%LINK%%[[#^h1bp4hlit4d|show annotation]]
>%%COMMENT%%
>Set sigma 3 to be 0 and multiply back with the two rotation matrix for F'. This is the closest matrix that is rank 2 matrix (in general n-k matrix).
>%%TAGS%%
>
^h1bp4hlit4d


>%%
>```annotation-json
>{"created":"2024-02-10T01:53:19.749Z","text":"If we had 7 points it would be under-constrained because we would need to a polynomal -> outside of linear algebra.","updated":"2024-02-10T01:53:19.749Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":8466,"end":8544},{"type":"TextQuoteSelector","exact":"F has 7 degrees of freedom, but use            to be able to use linear method","prefix":"y dropping last singular value• ","suffix":" 0=AfAfGiven n point corresponde"}]}]}
>```
>%%
>*%%PREFIX%%y dropping last singular value•%%HIGHLIGHT%% ==F has 7 degrees of freedom, but use            to be able to use linear method== %%POSTFIX%%0=AfAfGiven n point corresponde*
>%%LINK%%[[#^s8840ncab8a|show annotation]]
>%%COMMENT%%
>If we had 7 points it would be under-constrained because we would need to a polynomal -> outside of linear algebra.
>%%TAGS%%
>
^s8840ncab8a


>%%
>```annotation-json
>{"created":"2024-02-10T02:05:18.376Z","text":"Matches should be consistent","updated":"2024-02-10T02:05:18.376Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":9409,"end":9483},{"type":"TextQuoteSelector","exact":"Points in correspondence should be consistent with some fundamental matrix","prefix":" as a model to remove outliers• ","suffix":"• Find the fundamental matrix wi"}]}]}
>```
>%%
>*%%PREFIX%%as a model to remove outliers•%%HIGHLIGHT%% ==Points in correspondence should be consistent with some fundamental matrix== %%POSTFIX%%• Find the fundamental matrix wi*
>%%LINK%%[[#^6ou81e6mi18|show annotation]]
>%%COMMENT%%
>Matches should be consistent
>%%TAGS%%
>
^6ou81e6mi18


>%%
>```annotation-json
>{"created":"2024-02-10T02:08:05.305Z","text":"We pick two random points, get a line, and see how many points are roughly close enough. In this case there are 3 in consensus.","updated":"2024-02-10T02:08:05.305Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":9710,"end":9728},{"type":"TextQuoteSelector","exact":": Counting Inliers","prefix":"mohan ChandrakerInliers: 3RANSAC","suffix":"CSE 152A, WI24: Manmohan Chandra"}]}]}
>```
>%%
>*%%PREFIX%%mohan ChandrakerInliers: 3RANSAC%%HIGHLIGHT%% ==: Counting Inliers== %%POSTFIX%%CSE 152A, WI24: Manmohan Chandra*
>%%LINK%%[[#^66t1rx896y5|show annotation]]
>%%COMMENT%%
>We pick two random points, get a line, and see how many points are roughly close enough. In this case there are 3 in consensus.
>%%TAGS%%
>
^66t1rx896y5


>%%
>```annotation-json
>{"created":"2024-02-10T02:09:11.255Z","text":"Random sample consensus","updated":"2024-02-10T02:09:11.255Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":9833,"end":9839},{"type":"TextQuoteSelector","exact":"RANSAC","prefix":" 152A, WI24: Manmohan Chandraker","suffix":"•General version:1. Randomly cho"}]}]}
>```
>%%
>*%%PREFIX%%152A, WI24: Manmohan Chandraker%%HIGHLIGHT%% ==RANSAC== %%POSTFIX%%•General version:1. Randomly cho*
>%%LINK%%[[#^0nfaz5jmvhc9|show annotation]]
>%%COMMENT%%
>Random sample consensus
>%%TAGS%%
>
^0nfaz5jmvhc9


>%%
>```annotation-json
>{"created":"2024-02-10T02:13:11.780Z","text":"For all corrispondences","updated":"2024-02-10T02:13:11.780Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":10235,"end":10286},{"type":"TextQuoteSelector","exact":"Count number of inliers with             close to 0","prefix":"  using these 8 correspondences–","suffix":"•Pick the     with the largest n"}]}]}
>```
>%%
>*%%PREFIX%%using these 8 correspondences–%%HIGHLIGHT%% ==Count number of inliers with             close to 0== %%POSTFIX%%•Pick the     with the largest n*
>%%LINK%%[[#^ty2nw3cw3hd|show annotation]]
>%%COMMENT%%
>For all corrispondences
>%%TAGS%%
>
^ty2nw3cw3hd


>%%
>```annotation-json
>{"created":"2024-02-10T02:14:04.969Z","text":"We pick a threshold for inliers and outliers","updated":"2024-02-10T02:14:04.969Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":10327,"end":10334},{"type":"TextQuoteSelector","exact":"inliers","prefix":"     with the largest number of ","suffix":"FxT1Fx2CSE 152A, WI24: Manmohan "}]}]}
>```
>%%
>*%%PREFIX%%with the largest number of%%HIGHLIGHT%% ==inliers== %%POSTFIX%%FxT1Fx2CSE 152A, WI24: Manmohan*
>%%LINK%%[[#^owpl2o4m72c|show annotation]]
>%%COMMENT%%
>We pick a threshold for inliers and outliers
>%%TAGS%%
>
^owpl2o4m72c


>%%
>```annotation-json
>{"created":"2024-02-10T02:15:59.007Z","text":"Why are we working with minimal? Suppose we are given K matches across 2 images. Model has m degrees of freedom so we need m+1 samples. For k matches if we want the number of m+1 samples. K choose m1 samples. Suppose there is m2 matches. Suppose m1 > m2. Then kCm1 > kCm2. O(k^m1) vs O(k^m2). Drawing more samples gets expensive so thats why we want the minimal sample given the # of degrees of freedom.","updated":"2024-02-10T02:15:59.007Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":10217,"end":10234},{"type":"TextQuoteSelector","exact":"8 correspondences","prefix":"es–Estimate an      using these ","suffix":"–Count number of inliers with   "}]}]}
>```
>%%
>*%%PREFIX%%es–Estimate an      using these%%HIGHLIGHT%% ==8 correspondences== %%POSTFIX%%–Count number of inliers with*
>%%LINK%%[[#^rtsxazbw58|show annotation]]
>%%COMMENT%%
>Why are we working with minimal? Suppose we are given K matches across 2 images. Model has m degrees of freedom so we need m+1 samples. For k matches if we want the number of m+1 samples. K choose m1 samples. Suppose there is m2 matches. Suppose m1 > m2. Then kCm1 > kCm2. O(k^m1) vs O(k^m2). Drawing more samples gets expensive so thats why we want the minimal sample given the # of degrees of freedom.
>%%TAGS%%
>
^rtsxazbw58


>%%
>```annotation-json
>{"created":"2024-02-10T02:22:16.021Z","text":"p is probability of getting right solution. s is the model size (degrees of freedom). epsilon (proportion of expected outliers). if p = 0.99, 8 point agorithm. If we expect 25% are corrupted, we need 44 random draws of 8 points we can get a 99 percent probability of arriving at the right fundemental matrix.\n","updated":"2024-02-10T02:22:16.021Z","document":{"title":"lec09_twoview.pdf","link":[{"href":"urn:x-pdf:6ba9617c847aa100dcd873371b374e4a"},{"href":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf"}],"documentFingerprint":"6ba9617c847aa100dcd873371b374e4a"},"uri":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","target":[{"source":"https://cseweb.ucsd.edu/~mkchandraker/classes/CSE152A/Winter2024/Lectures/lec09_twoview.pdf","selector":[{"type":"TextPositionSelector","start":10422,"end":10491},{"type":"TextQuoteSelector","exact":"Adaptively determine number of iterations based on outlier proportion","prefix":"imate Fundamental MatrixRANSAC• ","suffix":"Values of N for p = 0.99CSE 152A"}]}]}
>```
>%%
>*%%PREFIX%%imate Fundamental MatrixRANSAC•%%HIGHLIGHT%% ==Adaptively determine number of iterations based on outlier proportion== %%POSTFIX%%Values of N for p = 0.99CSE 152A*
>%%LINK%%[[#^fhkrgvnjoe6|show annotation]]
>%%COMMENT%%
>p is probability of getting right solution. s is the model size (degrees of freedom). epsilon (proportion of expected outliers). if p = 0.99, 8 point agorithm. If we expect 25% are corrupted, we need 44 random draws of 8 points we can get a 99 percent probability of arriving at the right fundemental matrix.
>
>%%TAGS%%
>
^fhkrgvnjoe6
