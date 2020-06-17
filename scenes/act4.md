# act4

```
SceneSetup.act4();
publish("SAVE_GAME", ["act4"]);
Game.FORCE_CANT_SKIP = true;
```

(...5001)

```
publish("set_how_many_prompts", [1]);
Game.FORCE_CANT_SKIP = false;
Game.CLICK_TO_ADVANCE = true;
```

n3: (trò chơi đã tự động lưu)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
var hong_frame = _.INJURED ? 9 : 0;
publish("act4", ["hong_walks_in",hong_frame]);
sfx("grass_step1", {volume:0.1});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.2});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.25});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.3});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...1667)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...1333)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.20});
```

(...167)

```
publish("act4_hong_sits");
```

(...66)

```
publish("act4", ["hong_transition", "next"]);
sfx("squeak");
```

(...133)

`publish("act4", ["hong_transition", "next"]);`

(...1333)

```
publish("act4", ["hong_transition", "next"]);
sfx("rustle");
```

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1001)

```
publish("act4", ["hong_transition", "next"]);
```

(...333)

```
publish("act4", ["hong_transition", 9]);
sfx("sandwich");
```

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1466)

`publish("act4-out-1");`

(...201)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

```
publish("act4-show-chars");
Game.FORCE_CANT_SKIP = false;
```

(...901)

`hong({body:"sigh_1"})`

(...601)

```
hong({body:"sigh_2"});
bb({eyes:"look_down"});
```

h: *hầy*

```
hong({body:"hold", eyes:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Vậy câu chuyện này đã dạy cho chúng ta bài học ^chết tiệt^ gì thế?

`hong({body:"one_up", eyes:"annoyed"})`

h: Thậm chí chúng ta đã *học* được gì?! Tôi *là* đứa ngu ngốc, "bạn" tôi *đang* lợi dụng tôi, và chúng ta mém *chết* à.

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[Ừa, còn chưa đề cập đến tiền viện phí nữa.](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[Ừa, còn chưa đề cập đến việc gan bị tàn phá nữa.](#act4a_liver)
{{/if}}

[Ừa, kịch bản đó *cũng* tồi tệ khiếp đấy.](#act4a_worst)

[Ừa, tôi đã đúng.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: Ừa. Thật may là có bảo hiểm y tế.

`hong({eyes:"annoyed", mouth:"normal"});`

b: Dù thế... chúng ta vẫn sống sót!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: Cứ xác định là chúng ta vừa mất đi vài năm tuổi thọ ha...

`bb({eyes:"surprise"});`

b: Nhưng ít nhất chúng ta vẫn *có* tuổi thọ! Chúng ta vẫn sống!

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ?

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: Dù thế...

h: Hửm?

`bb({eyes:"surprise"});`

b: Chúng ta vẫn sống!

(#act4b)

# act4a_right

`bb({eyes:"normal_d"});`

b: Nhưng... cậu cũng đúng.

`hong({eyes:"surprise"});`

h: Hửm?

`bb({eyes:"normal"});`

b: Tôi *chỉ* là một con sói xấu xa. Nên khi cậu *thực sự* đối mặt với nguy hiểm, cậu - nói thẳng ra - là đừng tin tôi.

`bb({eyes:"surprise_r"});`

b: Dù thế, chúng ta vẫn sống!

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: Mặc kệ mọi thứ, chúng ta vẫn ở đây.

`hong({eyes:"suspect"});`

{{if _.INJURED}}
h: Trông cậu khá bình tĩnh nhỉ, dù cho chúng ta vừa mới được trải nghiệm cảm giác cận tử ha.
{{/if}}

{{if !_.INJURED}}
h: Trông cậu khá bình tĩnh nhỉ, dù cho chúng ta vừa mới được trải nghiệm cảm giác *cận* cận tử ha.
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: Ừm, nếu so sánh thì mọi thứ cũng không quá đáng sợ so với việc đấy. Với lại, nhờ thế mà tôi bắt đầu suy nghĩ thế này.

`bb({eyes:"normal", mouth:"normal"});`

b: Tôi đã làm những điều tồi tệ với cậu, chẳng thể nào bảo vệ được cậu...

h: Tôi *cũng* đã làm những điều tồi tệ với cậu, khiến cậu gào thét nhiều hơn...

`bb({eyes:"normal_r"})`

b: Vậy thì có lẽ...

`bb({eyes:"normal"})`

h: Có lẽ chúng ta không cần phải chiến đấu nữa.

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
```

(...301)

`publish("smash",[0]);`

(...2001)

```
publish("smash",[1]);
sfx("smash_glass");
```

(...2601)

```
publish("smash",[2]);
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

(...2001)

`Game.FORCE_CANT_SKIP = false;`

(#act4b_2)

# act4b_2

```
music('dontfight',{fade:5, volume:0.6});
bb({eyes:"annoyed_d"});
```

b: Tôi không phải con Sói lớn xấu xa.  Tôi cũng không phải là một chú sói bảo vệ.

`bb({eyes:"sad_d"})`

b: Tôi chỉ là một chú chó đi lạc bị hành hạ.

`bb({eyes:"sad"})`

b: Chúng ta trải qua nhiều điều tồi tệ, chịu tổn thương tâm lí hoặc bị thờ ơ. Đó là lí do tại sao đôi khi tôi lại phản ứng thái quá và:

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: GÂU GÂU GÂU GÂU GÂU

(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: Nhưng tôi không *muốn* làm một chú chó hèn nhát! Tôi muốn bảo vệ cậu! Tôi muốn làm một chú chó ngoan!

`bb({eyes:"sad", mouth:"normal"});`

b: Con người à... cậu sẽ thuần hóa chú sói này chứ?

`hong({eyes:"sad"})`

h: Tôi... Tôi sẽ cố gắng.

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: Được rồi. Mối quan hệ lành mạnh với cảm xúc nhé. Mà mối quan hệ thì cần giao tiếp. Nên hãy giao tiếp nào.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: Có thể 5 phút kế tiếp sẽ có hơi đạo đức giả một chút, nhưng chúng ta vẫn phải giả vờ cho đến khi đạt được mục tiêu.

```
hong({body:"hands_2", mouth:"normal"});
```

h: Chú sói nội tâm thân mến... *cậu* cảm thấy thế nào?

n2: TỔNG NỖI SỢ ĐÃ DÙNG:

n2: *BỊ TỔN HẠI* {{_.attack_harm_total}}, *KHÔNG ĐƯỢC YÊU* {{_.attack_alone_total}}, *LÀM NGƯỜI XẤU* {{_.attack_bad_total}}

n2: BẠN MUỐN NÓI VỀ NỖI SỢ NÀO TRƯỚC? (BẠN CÓ THỂ NÓI VỀ NHỮNG NỖI SỢ KHÁC SAU)

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[Tôi sợ chúng ta sẽ bị tổn hại.](#act4_harm)

[Tôi sợ chúng ta sẽ đơn độc.](#act4_alone)

[Tôi sợ chúng ta sẽ trở thành người xấu.](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: Tôi muốn bảo vệ sự an toàn cho nhu cầu thể chất của cậu,

`bb({eyes:"sad_d"})`

b: Nhưng *cả thế giới này* chỉ toàn là sự nguy hiểm. Tràn ngập bi kịch và sự độc ác.

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: Tôi không biết nữa, nhưng *tôi* nghĩ mình nói đủ rồi. Còn *cậu* thì sao hở, con người?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Vậy còn cậu, cậu nghĩ gì hở con người?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Ý cậu thì sao, con người?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Cậu nói đúng. Hãy bảo vệ lẫn nhau nào.](#act4_harm_skills)

[Hãy thử dùng liệu pháp tiếp xúc với những điều nguy hiểm *hơn* nào.](#act4_harm_exposure)

[Cảm ơn cậu.](#act4_thanks) `_.thanks_for = "sự an toàn thể chất";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: Nhưng... bằng cách nào? Tôi có móng và vuốt, nhưng tôi cũng chỉ là một phép ẩn dụ mà thôi.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: Chúng ta có thể học cách tự bảo vệ bản thân mà? Tham gia vào một cộng đồng bảo vệ lẫn nhau thì sao nhỉ? Hay cải thiện sức khỏe cũng như khoảng cách xã hội của chúng ta?

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: Có lẽ thế, nhưng...

[Chúng ta nên bắt đầu từ đâu?](#act4_harm_skills_start)

[Lỡ như chúng không có ích thì sao?](#act4_harm_skills_work)

[Lỡ như chúng ta quá tập trung vào "sự an toàn" thì sao?](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: Có nhiều điều cần phải làm, nhiều thứ chúng ta cần phải khắc phục. Chúng ta phải *bắt đầu* từ đâu?

`hong({ body:"shrug", eyes:"surprise" })`

h: Chúng ta đang bắt đầu đấy thôi.

`bb({ eyes:"normal", mouth:"narrow" })`

b: Ể?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: Chúng ta đang học cách để giao tiếp tốt với mọi người mà. Việc đó sẽ giúp chúng ta nhận ra sự nguy hiểm tốt hơn,

`hong({ eyes:"surprise" });`

h: Và *như vậy* việc đó sẽ bảo vệ chúng ta khỏi sự tổn hại!

`hong({ eyes:"normal", mouth:"normal" });`

h: Vì vậy: đây *chính là* đào tạo tự bảo vệ bản thân.

`bb({ eyes:"normal_r" })`

b: Hừm. Tôi còn trông đợi nhiều hơn thế đấy.

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
hong({ eyes:"sad", mouth:"smile" });
bb({ body:"karate_1" });
sfx("hiya");
```

(...1001)

`Game.FORCE_CANT_SKIP = false;`

(#act4_something_else)

# act4_harm_skills_work

`bb({ eyes:"normal" });`

h: Đúng vậy, chẳng có cách nào bảo vệ chúng ta 100% khỏi sự nguy hiểm cả...

`hong({ body:"one_up" });`

h: Nhưng cải thiện được 1% thì cũng xứng đáng mà, đúng không?

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: Dù cho ly thủy tinh đó rỗng đến 99%, cậu vẫn có thể nói nó có 1% nước mà ha?

`bb({ eyes:"normal" });`

h: Điều đó vẫn đáng giá nếu cậu bị mắc kẹt trong sa mạc.

`bb({ eyes:"closed" });`

b: Okei, tôi đồng ý.

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: Ý tôi là, toàn bộ lí do cậu phớt lờ lời cảnh báo của tôi có lẽ vì *tôi* quá tập trung vào sự an toàn!

`bb({ body:"normal", eyes:"normal" })`

h: Nầu, cậu đúng mà. Chúng ta luôn muốn được kiểm soát sự an toàn mà. Mọi thứ đều trong tầm kiểm soát.

`bb({ eyes:"suspect" })`

b: Xin lỗi, *MỌI THỨ* trong tầm kiểm soát ấy?

`hong({ eyes:"annoyed" })`

h: *Một vài việc ở mức vừa phải* trong tầm kiểm soát.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: Cảm ơn vì cậu đã làm rõ điều đó.

(#act4_something_else)

# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *SAO CƠ*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: Ý tôi là, có thể nói rằng chó cũng sợ sấm sét.

`hong({ body:"hands_1" });`

h: Một mẹo huấn luyện thường được dùng là phát một bản ghi tiếng sấm ở âm lượng thấp, rồi sau đó chăm sóc chú chó đó, khiến nó bình tĩnh trở lại.

`hong({ body:"hands_2" });`

h: Qua nhiều ngày sau, người huấn luyện tăng dần âm lượng, từng chút từng chút một, cho đến khi chú chó ấy vượt qua được nỗi sợ tiếng sấm.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: Đó được gọi là liệu pháp tiếp xúc!

`hong({ body:"point", eyes:"normal" });`

h: Vì cậu là chó nên như vậy cũng sẽ có tác dụng mà nhỉ? Tất cả các loài động vật có vú khác đều có cùng Phản ứng Chiến-hay-Chạy như nhau mà.

`hong({ body:"normal" });`

[Lỡ như chúng ta bị mất luôn cảm thụ thì sao?](#act4_harm_exposure_overboard)

[Lỡ như chúng ta đối mặt với nguy hiểm *thật sự* luôn thì sao?](#act4_harm_exposure_hurt)

[Tôi là sói, không phải chó.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: Và tôi sẽ tốt bụng và kiên nhẫn với cậu, cho đến khi thuần hóa cậu thành một chú cún dễ thương.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: Ư ư.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: Chúng ta *chỉ* thấy được những gì xảy ra khi cậu mất đi nỗi sợ - cậu đã đặt bản thân mình vào một tình huống nguy hiểm *thật sự*.

`bb({ eyes:"angry_r", body:"one_up" })`

b: Bên cạnh đó, nếu không quá nhạy cảm chúng ta sẽ biến thành những kẻ đa nhân cách đúng không?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: Sớm muộn gì chúng ta cũng sẽ biến thành loại người ngồi ăn bỏng ngô trong khi đang xem phim khiêu dâm giết người kinh tởm!

`hong({ eyes:"annoyed" })`

h: Tôi... nghĩ rằng việc đó khác hoàn toàn với sấm sét.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: Nhưng chính xác thì nó *ở đâu* hở con người? *Ở đâu?!*

`hong({ eyes:"surprise", body:"one_up" })`

h: Tôi không biết. Nhưng *cậu* có thể giúp tôi!

`hong({ eyes:"normal", body:"normal" })`

h: Trong khi làm việc và đàm phán với cậu, chúng ta sẽ vẽ ra làn ranh ngăn cách thứ đó.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: Được rồi. Nhưng tôi không có ngón tay cái, nên cậu phải vẽ chúng đấy.

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: Ví dụ: chúng ta nhảy xuống từ cái *mái nhà* chết tiệt đấy!
{{/if}}

{{if !_.INJURED}}
b: Ví dụ: chúng ta mém nhảy xuống từ cái *mái nhà* chết tiệt đấy!
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: Ừa cậu nói đúng. Đôi khi mọi thứ có thể vượt quá tầm kiểm soát.

`hong({ eyes:"normal" });`

h: Nhưng đó chính là lí do, chúng ta sẽ dùng liệu pháp tiếp xúc, chúng ta sẽ thông minh hơn, rồi chúng ta sẽ tiến xa hơn từng bước từng bước.

h: Và dừng lại ngay trước khi chúng ta đối mặt với nguy hiểm *thật sự*.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: Ừa, tôi sẽ vẽ ra làn ranh giữa việc nghe thấy tiếng sấm, và việc đứng giữa một cơn bão trong khi đang đổi một chiếc mũ nhọn cao. 

(#act4_something_else)

# act4_thanks

`_.num_thanks += 1`

{{if _.num_thanks==1}}
(#act4_thanks_1)
{{/if}}

{{if _.num_thanks==2}}
(#act4_thanks_2)
{{/if}}

{{if _.num_thanks==3}}
(#act4_thanks_3)
{{/if}}

# act4_thanks_1

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"annoyed" })`

b: Khoan đã, cậu không định tranh cãi hay phản đối cảm xúc của tôi sao? Chỉ... "cảm ơn" thôi à?

`hong({ eyes:"surprise", body:"shrug" })`

h: Ừa! Cảm ơn vì đã quan tâm đến {{_.thanks_for}} của tôi.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: Cậu ổn chứ?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: Trước giờ cậu chưa hề nói *cảm ơn* với tôi.

`hong({ mouth:"smile" });`

h: Aw đồ con sói to lớn lông xù đáng thương.

(#act4_something_else)

# act4_thanks_2

h: Dù cho cậu có phản ứng thái quá, tôi vẫn biết ơn vì cậu đã quan tâm đến {{_.thanks_for}} của tôi.

`bb({ eyes:"annoyed" })`

b: Chờ đã... chắc không phải cậu lặp lại lời "cảm ơn" chỉ để tránh nhắc đến nỗi sợ của bản thân nhỉ?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: Ừm, mấy thứ đó vô cùng rắc rối, và không phải lúc nào tôi cũng có sẵn câu trả lời.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: Cuộc sống này không cho cậu chọn 3 đoạn hội thoại được tạo sẵn đâu.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: Nhưng giờ đây, ít nhất tôi cũng có thể nói cảm ơn.

b: Ừa, tôi cũng cảm ơn cậu, vì đã kiên nhẫn lắng nghe tôi.

`bb({ eyes:"closed" });`

b: Đồ động vật trụi lông nhỏ bé.

(#act4_something_else)

# act4_thanks_3

h: Dù cho những điều cậu làm khiến tôi sợ, cậu đơn giản chỉ muốn bảo vệ {{_.thanks_for}} của tôi thôi.

`bb({ eyes:"smile_r" });`

b: Được rồi, nếu cậu cứ tiếp tục tâng bốc tôi như thế, cư dân mạng sẽ lại bắt đầu lòi ra mấy ý tưởng kì lạ về chúng ta đấy.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: Thôi nào, tôi chỉ là một đứa nhóc sinh viên đại học mong manh nhỏ bé, còn cậu là một chú sói to lớn đáng sợ mà. Điều tồi tệ gì có thể xảy ra--

`hong({ eyes:"normal", body:"point" });`

h: Thật sự thì, không cần trả lời điều đó đâu.

(#act4_something_else)

# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: Tôi chỉ muốn cậu có được cảm giác thân thuộc mà thôi...

`bb({ eyes:"sad_u" });`

b: Nhưng tôi sợ rằng nếu có ai đó biết đến chúng ta – bản chất *thật sự* – chúng ta sẽ dọa họ chạy mất.

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: Tôi không biết nữa, nhưng *tôi* nghĩ mình nói đủ rồi. Còn *cậu* thì sao hở, con người?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Vậy còn cậu, cậu nghĩ gì hở con người?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Ý cậu thì sao, con người?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Tôi đồng ý: hãy tiếp tục cố gắng nào.](#act4_alone_skills)

[Tôi nghĩ người khác sẽ thích chúng ta thôi. Cố gắng cùng nhau nhé?](#act4_alone_experiment)

[Cảm ơn cậu.](#act4_thanks) `_.thanks_for = "vấn đề xã hội";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: Chúng ta có thể luyện tập kĩ năng như đặt ra những câu hỏi, lắng nghe và đồng cảm, hay cởi mởi và dễ bị tổn thương hơn nhỉ?

`hong({ eyes:"normal_l" });`

h: Hoặc tạo nên những thói quen xã hội tốt hơn, như sắp xếp thời gian đi chơi cùng bạn bè hay gặp gỡ người khác ha?

`hong({ body:"one_up" });`

h: Như vậy chúng ta cũng có thể học cách thoải mái hơn khi bị từ chối.

`hong({ eyes:"normal" });`

h: Hoặc xác định được rằng người khác *không phải* đang từ  chối chúng ta, chỉ là họ đang mệt mỏi, hoặc mặt họ vốn dĩ đã như thế.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: Có thật nhiều lựa chọn. Nhưng, về việc "học những kĩ năng xã hội"...

[Không phải như thế là *thao túng* người khác à?](#act4_alone_skills_manipulative)

[Việc đó khiến chúng ta *dễ bị thao túng* hơn à?](#act4_alone_skills_manipulated)

[Lỡ như chúng ta vẫn thất bại thì sao?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: Không phải những tên giết người hàng loạt có thể đọc được cảm xúc của nạn nhân luôn giỏi ở việc "đồng cảm" sao?

`bb({ eyes:"annoyed" });`

b: Không phải Charles Manson đã có được bạn bè và khiến người khác chú ý đến mình sao?

`hong({ eyes:"annoyed", body:"chin" });`

h: Không, cậu nói đúng.

h: "Kĩ năng xã hội" chẳng có ý nghĩa gì nếu chúng ta không quan tâm *đến* người khác.

`hong({ body:"normal" });`

h: Chỉ là, đừng hành xử như con ^c^ là được.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: Câu đó truyền cảm hứng tốt lắm đấy.

`hong({ body:"shrug", mouth:"narrow" });`

h: “Đừng Hành Xử Như Con ^C^™”

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: Chúng ta sẽ trở thành một tấm thảm ngoài cửa, nói Cảm Ơn khi người khác dẫm chân lên mặt chúng ta!

`bb({ mouth:"scream", eyes:"scream" })`

b: Chúng ta sẽ phải hôn mông họ, rồi mặt chúng ta sẽ trông giống như đang dùng son màu nâu!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: Không, cậu nói đúng. "Kĩ năng xã hội" không chỉ để làm hài lòng người khác, mà còn để lập ra *ranh giới*.

`hong( body:"one_up" });`

h: Chúng ta không thể mời người khác vào nhà, nếu như ngôi nhà của chúng ta không có tường bảo vệ.

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: Với lại...  son môi màu nâu á?... *eww??*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: Chúng ta có thể thất bại. Sự thật thì, chúng ta *sẽ* thất bại.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: Và điều đó ổn mà! Khi bắt đầu học một điều gì đó mới mẻ, chúng ta luôn có thể vấp ngã!

`hong({ body:"normal", eyes:"normal" });`

h: Vậy nên hãy thất bại, và tiếp tục tiến về phía trước cùng nhau nhé?

`bb({ eyes:"normal_r" });`

b: Ừa, chắc thế... trong trường hợp tồi tệ nhất, chúng ta có thể bỏ chạy và thay đổi danh tính mà ha.

`bb({ eyes:"normal" });`

h: Ừa, trong thời đại này chắc cần 2 bitcoin là đủ rồi.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Chúng ta có thể thử thí nghiệm mà!

`hong({ body:"chin" });`

h: Chúng ta có thể rủ bạn bè đi chơi, hẹn gặp những người bạn cũ, hay chỉ đơn giản là trò chuyện cùng nhân viên pha chế.

`hong({ body:"normal" });`

h: Có thể chúng ta thu hút hơn chúng ta nghĩ đấy.

`bb({ eyes:"annoyed" });`

[Lỡ như tỉ lệ của việc đó vô cùng nhỏ thì sao?](#act4_alone_experiment_cheap)

[Lỡ như việc này là gánh nặng của người khác thì sao?](#act4_alone_experiment_burden)

[Nhưng chỉ trò chuyện thôi thì vẫn chưa đủ!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: Nếu lúc nào chúng ta cũng trưng ra bộ mặt u sầu, thì chẳng bao giờ chúng ta có thể kết nối được với ai cả,

`bb({ eyes:"super_sad" });`

b: *Nhưng* nếu chúng ta cởi mở hơn, người khác có thể hiểu hơn về chúng ta!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Lăn đi.

b: Sao cơ.

`hong({body:"hands_1"})`

h: Khi chó muốn thể hiện tình yêu và sự tin tưởng, chúng sẽ để lộ bụng và khiến bản thân dễ bị tổn thương.

`hong({body:"one_up"})`

h: Có thể chúng ta vẫn còn yếu đuối, nhưng nếu chúng ta tập luyện nhiều hơn,

`hong({body:"normal", eyes:"surprise"})`

h: Một ngày nào đó, chúng ta sẽ có thể cho mọi người thấy chúng ta thực sự là ai - một con người hỗn loạn.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: Tôi sẽ lăn người nếu cậu thưởng cho tôi.

`bb({ eyes:"normal", mouth:"normal" });`

h: Không.

(#act4_something_else)

# act4_alone_experiment_cheap

b: Nói "chào" với người pha chế không giúp chúng ta có được huy chương vàng của giải Người Giao Thiệp Rộng Olympic đâu.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Việc này là vì *chúng ta*!

`hong({ body:"one_up", eyes:"annoyed" });`

h: Trong đấu trường xã hội, thậm chí chúng ta còn chẳng phù hợp với những hạng cân khác. Kiểu như chúng ta... là hạng cân quark.

`hong({ body:"normal", eyes:"normal" });`

h: Nếu bắt đầu từ những việc nhỏ nhất, thì cứ tới thôi. Phải trèo được bước đầu tiên thì mới đến được bước thứ 1000 chứ.

b: Ừa! Có lẽ sau khi nói "Chào", chúng ta có thể tiếp tục nói gì đó...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"Cậu khỏe chứ?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"Không khỏe lắm!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Có lẽ những người pha chế chỉ muốn pha cà phê, thay vì trở thành một *vật thí nghiệm* để xem kĩ năng xã hội của chúng ta tệ đến mức nào.

`bb({ eyes:"annoyed" })`

h: Ừm, nếu chúng ta *thực sự* trở thành gánh nặng...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Như thế cũng tốt mà!

`hong({ eyes:"normal" });`

h: Chúng ta có thể học cách chủ động hỏi thăm mọi người, biết được họ thoải mái với điều gì, và tôn trọng ranh giới của họ.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Cậu biết đấy, mấy thứ "kĩ năng giao tiếp giữa mỗi người" được viết đầy trong mớ tài liệu tư vấn tâm lý mà.

(#act4_something_else)

# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: Tôi muốn bảo vệ nhu cầu đạo đức của cậu, khiến cậu trở thành một người tốt hơn,

`bb({ eyes:"sad_d" })`

b: Nhưng đến cuối cùng, về căn bản chúng ta đã... tan vỡ.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: Và đừng bảo rằng chúng ta *không* hỗn loạn. Chúng ta đã nhảy xuống từ trên *mái nhà* đấy.
{{/if}}

{{if !_.INJURED}}
b: Và đừng bảo rằng chúng ta *không* hỗn loạn. Chúng ta đã mém nhảy xuống từ trên *mái nhà* đấy.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: Tôi không biết nữa, nhưng *tôi* nghĩ mình nói đủ rồi. Còn *cậu* thì sao hở, con người?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Vậy còn cậu, cậu nghĩ gì hở con người?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Ý cậu thì sao, con người?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Chúng ta đã tan vỡ rồi nhỉ. Hãy sửa chữa bản thân nào.](#act4_bad_fix)

[Chúng ta đã tan vỡ rồi nhỉ. Hãy chấp nhận việc đó nào.](#act4_bad_accept)

[Cảm ơn cậu.](#act4_thanks) `_.thanks_for = "hạnh phúc đạo đức";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: Chúng ta có thể chậm rãi xây dựng những thói quen tốt hơn, đưa cuộc sống của chúng ta phát triển đúng hướng và đạt được giá trị,

`hong({body:"one_up"});`

h: Và nếu cần, chúng ta có thể nhờ đến những sự giúp đỡ chuyên nghiệp - một nhà trị liệu hoặc một tư vấn viên thì sao nhỉ.

`hong({body:"normal"});`

h: Luôn có cách để sữa chữa bản thân mình mà.

[Giả sử nếu chúng ta không thể sửa chữa được hết thì sao?](#act4_bad_fix_cant)

[Nếu như chúng ta sữa chữa *quá* nhiều thì sao?](#act4_bad_fix_too_much)

[Chúng ta không đủ khả năng để nhờ mấy người chuyên nghiệp đâu.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: Không, tôi nghĩ cậu đã nói đúng.

h: Chúng ta không thể sửa chữa được mọi thứ.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: Ahhh tôi biết mà lúc nào chúng ta cũng tan vỡ hết!

`hong({eyes:"surprise"});`

h: Nhưng ít nhất chúng ta sẽ *ít* tan vỡ hơn.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: Vết thương rồi sẽ lành theo thời gian, và sẽ để lại sẹo. Như vậy vẫn ổn mà.

`bb({eyes:"annoyed_r"});`

b: Tôi hiểu. Bên cạnh đó,

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: Sẹo *gợi cảm* thấy mồ.

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: Làm ơn đừng làm điều đó.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: Thừa nhận thế này thật kinh dị, nhưng... một phần trong tôi *muốn* giữ lại sự rối loạn này.

`bb({ eyes:"angry" })`

b: Ý tôi là, nếu không có nó, thì không phải *buồn chán* lắm sao?

`bb({ eyes:"sad_r", body:"one_up" })`

b: Không có nó, mọi thứ sẽ thật cũ kĩ và nhàm chán.

`bb({ eyes:"sad_u", body:"two_up" })`

b: Và không có nó, chúng ta sẽ không thể kết nối được với những người bạn cũng mắc sự rối loạn này đúng không?

`bb({ eyes:"sad", body:"chest" })`

b: Nếu như bản thân đã hoàn hảo, thì chúng ta không thể nào tiếp tục phát triển được nữa.

`hong({ MOUTH_LOCK:true })`

h: ...

h: Thậm chí nếu chúng ta sợ... "hãy vượt qua nỗi sợ"...

h: Tôi không nghĩ chúng ta có thể vượt qua nỗi sợ được đâu.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: Ừa đúng vậy! Phù! Thật là nhẹ nhõm!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "Bác sĩ, tôi thấy lo âu khi trả $100/giờ chỉ để nghe ông hỏi *cậu cảm giác thế nào?*"

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "Mm-hmm. Vậy cậu cảm giác thế nào?"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: Nầu, lo lắng như thế hợp lí mà.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: Và thật khốn nạn khi nhiều người chẳng thể nào chi trả nổi cho dịch vụ chăm sóc sức khỏe tinh thần.

`hong({ eyes:"normal", mouth:"normal" });`

h: Với lại, vẫn còn những lựa chọn rẻ hoặc miễn phí khác cơ mà:

`hong({ body:"chin" })`

h: Những nhóm hỗ trợ, trị liệu trực tuyến, hay trung tâm tư vấn học đường/xã hội phi lợi nhuận này...

`hong({ body:"hands_1" })`

h: Xây dựng những thói quen như thiền, ngủ đủ giấc, trò chuyện thường xuyên cùng bạn bè, học hỏi những điều mới mẻ...

`hong({ body:"hands_2" })`

h: Đến thư viện mượn một quyển sách về hỗ trợ tâm lí trị liệu...

`hong({ body:"one_up" })`

h: Có vô cùng nhiều cách luôn đấy! Và có rất nhiều người luôn sẵn sàng giúp đỡ các bạn!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: Ừm bức tường thứ tư *đấy* sẽ không tồn tại lâu đâu ha.

`hong({ body:"point" });`

h: Có nhiều thứ còn quan trọng hơn các tiêu chuẩn thường ngày. Như sức khỏe tinh thần chẳng hạn.

(#act4_something_else)

# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: Ý tôi là, đó là những điều mà mấy nhà trị liệu nói đúng không? Chấp nhận mọi cảm xúc, kể cả cảm xúc tiêu cực nhỉ?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: Chờ đã.

["Chấp nhận" có nghĩa là *từ bỏ* ấy?](#act4_bad_accept_give_up)

["Chấp nhận" có nghĩa là *chứng minh* ấy?](#act4_bad_accept_approve)

["Chấp nhận" *theo nghĩa đen* ấy?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: Cậu có nghĩ rằng Martin Luther King sẽ nói, "Trời ạ chúng ta không thể ngồi ở phía trước xe bus, đành *chấp nhận* điều đó thôi" không?

`bb({ eyes:"angry_r", body:"two_up" });`

b: Tại sao Khu phức hợp Tự giúp đỡ lại nghĩ rằng vẫy cờ trắng là một điều *khôn ngoan?*

`bb({ eyes:"annoyed", body:"normal" });`

h: Tôi nghĩ khi những nhà trị liệu nói rằng "chấp nhận" những điều xấu thì có nghĩa: thừa nhận sự tồn tại của chúng và chúng thật khó để thay đổi,

h: Nhưng điều này không có nghĩa chúng ta sẽ từ bỏ sự thay đổi.

`bb({ eyes:"suspect" });`

b: Vậy thì những nhà trị liệu nên nói là *thừa nhận*, không phải *chấp nhận*.

`hong({ body:"chin", eyes:"annoyed" });`

h: Ừa, nếu nghĩ thế thì "chấp nhận" có hơi khó hiểu một chút.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Ừm, tôi *thừa nhận* điều đó.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: Như kiểu thật *tốt* khi chúng ta bị tan vỡ à? Không!

`bb({ eyes:"angry_r", body:"one_up" });`

b: Những nhà biên kịch Hollywood đang lãng mạn hóa bệnh tâm lí đều là những tên độc ác!

`bb({ eyes:"angry", body:"two_up" });`

b: Mắc phải chứng rối loạn tinh thần thật *khốn nạn!* Nó đã cướp đi *cuộc sống* của rất nhiều người! Vậy tại sao chúng ta lại nên "chấp nhận" điều đó?!

`bb({ body:"normal" });`

h: Tôi nghĩ khi những nhà trị liệu nói rằng "chấp nhận" cảm xúc của chúng ta thì có nghĩa: hãy kiên nhẫn với chúng.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Như kiểu khi bị chìm trong cát lún và vùng vẫy chỉ khiến cậu chìm nhanh hơn, thì giải pháp ở đây là kiên nhẫn nằm thẳng,

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: Chiến đấu với cậu, nỗi sợ của tôi, đã khiến tôi nhảy xuống từ trên mái nhà.
{{/if}}

{{if !_.INJURED}}
h: Chiến đấu với cậu, nỗi sợ của tôi, đã khiến tôi mém nhảy xuống từ trên mái nhà.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: Thay vào đó, giải pháp cần thiết là điều chúng ta hiện đang làm - không phải chiến đấu, mà là kiên nhẫn với nhau.

`bb({ eyes:"annoyed" });`

b: Vậy thì họ nên nói *như vậy* thay vì dùng mấy từ rắc rối như "chấp nhận".

`hong({ body:"chin", eyes:"annoyed" });`

h: Ừa, nếu nghĩ thế thì "chấp nhận" có hơi khó hiểu một chút.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: Tôi không chấp nhận từ "chấp nhận".

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: Chứng chúng ta đều *biết* cậu không thể chấp nhận tôi theo nghĩa đen!

`bb({ eyes:"sad_u", body:"two_up" });`

b: Toàn bộ *vấn đề* ở đây là tôi muốn giúp cậu, nhưng tôi quá tệ ở khoảng biểu đạt!

`bb({ eyes:"sad", body:"normal" });`

h: Tôi nghĩ khi những nhà trị liệu nói rằng "chấp nhận" cảm xúc của cậu thì có nghĩa: "đừng chiến đấu hay phớt lờ chúng."

`hong({ eyes:"surprise", body:"one_up" });`

h: Lắng nghe cậu, làm việc *với cậu*, nhưng không hoàn toàn tin 100% những gì cậu nói là sự thật.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: Vậy thì họ nên nói *như vậy* thay vì dùng mấy từ rắc rối như "chấp nhận".

`hong({ body:"chin", eyes:"annoyed" });`

h: Tôi nghĩ họ cũng tệ ở khoảng dùng từ luôn.

(#act4_something_else)

# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: Dù sao thì, cậu còn muốn trò chuyện về điều gì nữa không?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: Vậy, còn điều gì khiến cậu nặng lòng nữa không?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[Tôi sợ chúng ta sẽ bị tổn hại.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[Tôi sợ chúng ta sẽ đơn độc.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[Tôi sợ chúng ta sẽ trở thành người xấu.](#act4_bad)
{{/if}}

[Không, bây giờ tôi ổn rồi.](#act4c_prelude)

# act4_something_else_2

h: Được rồi, tôi nghĩ chúng ta đã cùng nhau trò chuyện về tất cả nỗi sợ của chúng ta.

b: Ừa, chính xác chỉ có 3 nỗi sợ.

h: Ừm, chính xác chỉ có 3.

b: Thật tiện lợi.

(#act4c)

# act4c_prelude

h: Trò chuyện hay lắm, đồng đội à.

(#act4c)

# act4c

```
Game.clearText();
music(null,{fade:3});
bb({body:"normal", eyes:"normal", mouth:"normal", MOUTH_LOCK:true},0);
hong({body:"normal", eyes:"normal", mouth:"normal"},0);
```

b: ...

`hong({MOUTH_LOCK:true},0)`

h: ...

`bb({eyes:"annoyed_d"})`

b: Đây không phải một *trò chơi*, cậu biết mà.

`bb({eyes:"angry_d", body:"one_up"})`

b: Xây dựng một mối quan hệ lành mạnh với cảm xúc của bản thân không đơn giản như việc nhấp chuột trên màn hình đâu.

`bb({eyes:"sad", body:"normal"})`

b: Chúng ta *có thể* cố gắng cùng nhau không?

b: Chúng ta *có thể* làm việc với nhau, như một nhóm được chứ?

`hong({eyes:"sad", body:"one_up"})`

h: Ừm,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: X-xin lỗi cậu...

```
Game.clearText();
publish("act4-in-2");
music('campus', {volume:0.5, fade:1});
```

(...2101)

(#act4d)

# act4d

`Game.WORDS_HEIGHT_BOTTOM = 221;`

`publish("act4", ["alshire", 0]);`

a: C-cậ-cậu có phiền không nếu tôi ngồi đây ăn trưa cùng cậu?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *Đây* là crush của cậu à? Tại sao họ lại ngồi một mình ở đó như một tên giết người hàng loạt tâm thần thế?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: Hỏi crush của mình rằng có nên ngồi với họ không á? Như kiểu cậu đang *thèm khát* lắm ấy?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *Đây* là crush của cậu à? Chúng ta đang phá hoại sự yên bình và yên tĩnh của họ! Chúng ta là một gánh nặng!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: Y- Ý tôi là- là, nếu không được thì cũng ổn thôi, tôi chỉ...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Chờ đã, tớ có gặp cậu ở bữa tiệc không nhỉ?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Ừa, dĩ nhiên! Lại đây nào.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Xin lỗi, giờ đây tôi muốn yên tĩnh một chút.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Đúng rồi, cậu ngồi ở trên băng ghế! Ở bữa tiệc đầu tiên tớ tham gia...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Và hoảng loạn đến mức đấm vào mặt chủ bữa tiệc.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: Và hoảng loạn đến mức bỏ chạy và khóc.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Chờ đã con người, có lẽ chúng ta đang khiến họ thấy không thoải mái đấy.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: A, tớ không có ý làm cậu xấu hổ đâu!

`publish("act4", ["hong_to_alshire",4]);`

h2: Tớ chỉ đang cố tỏ ra thân thiện, chỉ vậy thôi.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: AHHHHH TÔI BIẾT MÀ! HỌ LÀ LOẠI NGUY HIỂM CÓ TÂM LÍ HOẢNG LOẠN!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: AAHHH ẤN TƯỢNG ĐẦU TIÊN CHÚNG TA TẠO RA LÀ "CHỨNG KIẾN CHẤN THƯƠNG CỦA TÔI"! CÓ NGHĨA HỌ GHÉT CHÚNG TA RỒI!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AAAHHH CHÚNG TA KHIẾN AI ĐÓ NHỚ LẠI MỘT VIỆC KHIẾN HỌ CHẤN THƯƠNG. SỰ HIỆN DIỆN CỦA CHÚNG TA TỔN THƯƠNG NGƯỜI KHÁC ĐẤY.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Chờ đã con người, trông họ có vẻ không thoải mái lắm.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: À, dĩ nhiên là không ép buộc rồi!

`publish("act4", ["hong_to_alshire", 4]);`

h2: Tôi chỉ nói thôi, nếu muốn thì cậu cứ ngồi đi.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: HỌ ĐANG *QUÁ* THÂN THIỆN! NHƯ TED BUNDY, KẺ GIẾT NGƯỜI HÀNG LOẠT!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: HỌ CHỈ TỎ RA TỐT BỤNG THÔI! CHẲNG AI *THẬT SỰ* MUỐN GẦN GŨI VỚI CHÚNG TA CẢ!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AHHH CHÚNG TA LUÔN KHIẾN NGƯỜI KHÁC THẤY NGẠI! CHÚNG TA LÀ RÁC RƯỞI CỦA TRÁI ĐẤT!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Chờ đã có người, có thể chúng ta khiến họ không thoải mái đấy.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: À, tôi không có ý thô lỗ đâu!

`publish("act4", ["hong_to_alshire", 6]);`

h2: Chỉ là tôi muốn dành một chút thời gian để kiểm soát cảm xúc của bản thân. Đừng nghĩ là tôi từ chối nhé.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: HỌ ĐANG PHẢI ĐỐI PHÓ VỚI CÁI THỨ SUY NGHĨ KINH TỞM GÌ THẾ?! HỌ MUỐN LÀM GÌ ĐỂ LẤP ĐẦY TRÁI TIM BỆNH HOẠN CỦA HỌ?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: CHÚNG TA ĐÃ BỊ TỪ CHỐI! SẼ CHẲNG AI YÊU CHÚNG TA NỮA!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: CHÚNG TA ĐÃ GIÁN ĐOẠN HỌ! GIỜ ĐÂY HỌ SẼ CHẤN THƯƠNG MÃI MÃI VÀ ĐẤY LÀ LỖI CỦA CHÚNG TA!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: CHẠY CHẠY CHẠY CHẠY CHẠY CHẠY CHẠY CHẠY CHẠY CHẠY CHẠY CHẠY CHẠY CHẠY CHẠY CHẠY

```
Game.clearText();
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["alshire", 10]);
sfx("pop");
```

(...1001)

```
publish("act4", ["alshire", 11]);
sfx("alshire_run");
```

(...2601)

```
publish("act4-out-3");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
```

(...1201)

`publish("act4-jumpcut-hong");`

h: Hờ. Lạ thật đấy. Không biết họ đang suy nghĩ gì nhỉ.

`publish("act4", ["hong_closer", 2]);`

h: Dù sao thì, lúc nãy cậu nói gì thế?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: Ư, tôi quên rồi? Thứ gì đó về làm việc cùng nhau như một nhóm chăng?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: Họ bảo rằng chúng ta nên "hòa giải" với cảm xúc của chính mình, như thể chúng là *tội phạm chiến tranh* vậy.

`publish("act4", ["bb_closer", 7]);`

b: Nhưng tôi muốn chúng ta đi xa *hơn* việc hòa giải! Tôi muốn chúng ta trở thành *đồng minh*!

`publish("act4", ["bb_closer", 3]);`

b: Tôi muốn trở thành một chú chó bảo vệ ngoan ngoãn. Như cách cơn đói và cơn khát cảnh báo cậu về nhu cầu thể chất,

`publish("act4", ["bb_closer", 8]);`

b: Tôi muốn cảnh báo cậu về nhu cầu *tâm lý* – nhu cầu an toàn, thân thuộc, và đạo đức của cậu.

`publish("act4", ["bb_closer", 1]);`

b: Nhưng... tôi chẳng giỏi việc này, nên tôi cần cậu huấn luyện tôi.

`publish("act4", ["bb_closer", 4]);`

b: Tôi không phải "luôn có giá trị," hay "luôn vô lý." Tôi chỉ là... cố gắng hết sức mình. Nên, làm ơn,

`publish("act4", ["bb_closer", 30]);`

b: Giúp tôi cũng là giúp cậu nhé!

`publish("act4", ["bb_closer", 6]);`

b: Dù vậy, dạy một chú chó già những kĩ năng mới *sẽ* mất một lúc. Có thể là *nhiều năm*.

`publish("act4", ["bb_closer", 3]);`

b: Và đôi khi tôi sẽ lại lặp lại những thói quen cũ.

`publish("act4", ["bb_closer", 2]);`

b: Tôi sẽ sủa với cái bóng. Tôi khiến cậu sợ hãi bằng ngôn từ. Thậm chí tôi có thể buộc cậu xem mấy hình ảnh... quấy rối.

`publish("act4", ["bb_closer", 9]);`

b: Tôi xin lỗi! Tôi chỉ là một chú chó đi lạc bị hành hạ! Một chú chó đi lạc đôi khi còn ị lên giường cậu!

`publish("act4", ["bb_closer", 4]);`

b: Nhưng nếu cậu kiên nhẫn với tôi... và ở đó bên cạnh tôi...

`publish("act4", ["bb_closer", 8]);`

b: Có lẽ cậu sẽ thuần hóa được chú sói này.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Chó ngoan.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[Con người ngoan.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

# act4f-pat-hong

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 13]);
```

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...6501)

`publish("act4", ["bb_closer", 15]);`

(...1001)

(#act4f)

# act4f-pat-bb

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 10]);
```

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...6501)

`publish("act4", ["bb_closer", 12]);`

(...1001)

(#act4f)

# act4f

```
Game.FORCE_CANT_SKIP = false;
publish("act4", ["bb_closer", 16]);
publish("act4", ["hong_closer", 5]);
```

{{if _.fifteencigs}}
b: AAAAA CẬU VẪN MỘT MÌNH ĂN MƯỜI LĂM ĐIẾU THUỐC AAAAA
{{/if}}

{{if _.parasite}}
b: AAAAA CẬU KHÔNG LÀM VIỆC HIỆU QUẢ KHI ĂN CHÚNG TA LÀ KÍ SINH XÃ HỘI AAAAA
{{/if}}

{{if _.whitebread}}
b: AAAAA CẬU LẠI ĂN THÊM BÁNH MÌ TRẮNG AAAAA
{{/if}}

```
publish("act4", ["bb_closer", 18]);
publish("act4", ["hong_closer", 6]);
sfx("yaps", {volume:0.6});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 205;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: GÂU GÂU GÂU GÂU GÂU

(#credits)
