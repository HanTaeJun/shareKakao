# shareKakao

* [Ko] 카카오톡 공유하기 모듈 (for Rhino)
* [En] Share Kakao Module (for Rhino)

![Alt text](sample/sample1.png)
![Alt text](sample/sample2.png)


# Warning
해당 모듈을 사용하여 얻는 모든 불이익에 대해 아무런 책임을 지지 않습니다.

> # Example
> ``` javascript
> const shareKakao = require("share.js");
> const Kakao = new shareKakao();
> Kakao.package("com.kakao.talk");
> ```
> 
> > * Share Simple Text
> > ``` javascript
> > Kakao.share("chat_id", {
> >     "type": 1,
> >     "message": "example",
> >     "attachment": {}
> > });
> >    ```
> 
> > * Share Shout Text
> > ``` javascript
> > Kakao.share("chat_id", {
> >     "type": 1,
> >     "message": "example",
> >     "attachment": {
> >         "shout": true
> >     }
> > });
> > ```
>
> > * Share Mention Text
> > ``` javascript
> > Kakao.share("chat_id", {
> >     "type": 1,
> >     "message": "@EliF -3-",
> >     "attachment": {
> >         "mentions": [{
> >             "at": [1],
> >             "len": 8,
> >             "user_id": "user_id"
> >         }]
> >     }
> > });
> > ```
>
> > * Share Simple Image
> > ``` javascript
> > Kakao.share("chat_id", {
> >     "type": 2,
> >     "message": "사진",
> >     "attachment": {
> >         "type": "image/jpeg",
> >         "w": 210,
> >         "h": 210,
> >         "path": "talkm/oXZBbblXG5/6VjK4Jl8OgLCiEfoFLS9V0/i_g9kyvd2sw3il.jpeg"
> >     }
> > });
> > ```
>
> # Available Types
> ``` javascript
> {
>     1: "text",
>     2: "image",
>     3: "video",
>     16: "map",
>     18: "file"
> }
> ```
