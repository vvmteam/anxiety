# act1

```
SceneSetup.act1();
```

(...300)

n: VÀ ĐÂY LÀ SỰ LO ÂU CỦA CON NGƯỜI

n: _BẠN_ LÀ SỰ LO ÂU ĐẤY

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}

# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: Ô này! Chúng ta quay lại đây rồi nhỉ?

`hong({eyes:"0_neutral"})`

n: CÔNG VIỆC CỦA BẠN LÀ BẢO VỆ CON NGƯỜI CỦA BẠN KHỎI *SỰ NGUY HIỂM*

`bb({eyes:"look", mouth:"small_lock"})`

n: SỰ THẬT LÀ, CHƠI LẠI TRÒ CHƠI NÀY ĐÃ KHIẾN HỌ GẶP *NGUY HIỂM* NGAY BÂY GIỜ RỒI

n: NHANH NÀO, CẢNH BÁO HỌ ĐI!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Con người! Nghe đây, chúng ta đang gặp nguy hiểm! Người chơi...

[...sắp hành hạ chúng ta nữa kìa!](#act1_replay_torture)

[...sẽ không thể tìm thấy một kết thúc thay thế đâu!](#act1_replay_alternate)

[...sẽ lại gặp mâu thuẫn giữa cốt truyện và cách chơi!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: Họ sẽ bắt chúng ta cuộn tròn lại thành một quả bóng và khóc!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: Họ sẽ khiến chúng ta phá hỏng điện thoại khi cậu hoảng loạn!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: Họ sẽ *KHÔNG* bắt chúng ta đấm chủ bữa tiệc!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: Họ sẽ bắt chúng ta đấm chủ bữa tiệc Phản đối Thông cảm!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: Ừm ít nhất lần này chúng ta sẽ không phải nhảy xuống từ mái nh--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: HỌ SẮP BẮT CHÚNG TA NHẢY XUỐNG TỪ MÁI NHÀ KÌA
{{/if}}

`bb({body:"fear"});`

b: TẤT CẢ NHỮNG ĐIỀU TỒI TỆ MỚI MẺ ĐÓ SẼ XẢY ĐẾN VỚI CHÚNG TA, VÀ RỒI CHÚNG TA SẼ--

(#act1_replay_end)

#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Đúng vậy, *cả* câu chuyện vẫn như thế thôi, nhưng mỗi chương có thêm hai kết thúc mới, cộng thêm một đống hội thoại bổ sung--

`bb({body:"fear"});`

b: Người chơi sẽ thất vọng, đóng tab trình duyệt này, xóa chương trình của chúng ta, rồi chúng ta sẽ--

(#act1_replay_end)

# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Thì sao?

`bb({eyes:"normal"});`

b: Câu chuyện này nói về cách cậu có thể *CHỌN* để xây dựng một sự hợp tác lành mạnh cũng nỗi sợ của cậu,

`bb({eyes:"normal_right"});`

b: Nhưng chơi lại trò chơi này cũng chỉ có nhiêu đó câu chuyện, ngụ ý rằng *LỰA CHỌN* của cậu chẳng còn quan trọng nữa,

`bb({eyes:"narrow_eyebrow"});`

b: Do đó có thể thấy được sự mâu thuẫn giữa thông điệp và cơ chế của trò chơi,

`bb({eyes:"fear"});`

b: Do đó cậu có thể thấy rõ kết cấu vũ trụ của câu chuyện này,

`bb({body:"fear"});`

b: Và sau đó chúng ta sẽ--

(#act1_replay_end)

# act1_replay_end

`bb({body:"panic"})`

b: CHẾTTTTTTTTTTTTTTTTT

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: Được rồi hãy quay lại câu chuyện nào.

```
Game.clearText();
```

n4: (HÃY ĐỂ SỰ LO ÂU _CỦA_ _BẠN_ THỂ HIỆN NHỮNG ĐIỀU TƯƠNG TỰ VỚI NỖI SỢ _CỦA_ _BẠN_ NÀO)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)

# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: Ồ tốt, chú sói của tôi quay lại rồi. Tuyệt vờiiiiii.

`hong({eyes:"0_neutral"})`

n: CÔNG VIỆC CỦA BẠN LÀ BẢO VỆ CON NGƯỜI KHỎI *SỰ NGUY HIỂM*

`bb({eyes:"look", mouth:"small_lock"})`

n: SỰ THẬT LÀ, CÁI SANDWICH ĐÓ ĐANG KHIẾN HỌ GẶP *NGUY HIỂM* NGAY LÚC NÀY

n: NHANH NÀO, CẢNH BÁO HỌ ĐI!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Con người! Nghe này, chúng ta đang gặp nguy hiểm! Điều nguy hiểm là...

`bb({body:"squeeze"})`

n4: (HÃY ĐỂ SỰ LO ÂU _CỦA_ _BẠN_ XUẤT HIỆN NÀO! CHỌN ĐIỀU TƯƠNG TỰ NHẤT VỚI ĐIỀU _BẠN_ SỢ NHÉ)

(#act1_normal_choice)

# act1_normal_choice

[Chúng ta đang ăn trưa một mình! Lại nữa!](#act1a_alone) `bb({body:"squeeze_talk"})`

[Chúng ta không làm việc hiệu quả trong khi ăn!](#act1a_productive) `bb({body:"squeeze_talk"})`

[Cái bánh mì trắng đó không tốt cho chúng ta!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: Cậu có biết việc cô đơn sẽ khiến cậu chết sớm vì nó có tác hại như hút 15 điếu thuốc mỗi ngày không?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Trong Holt-Lunstad 2010, PLoS Medicine đấy)

`hong({eyes:"0_annoyed"})`

h: Ừm, cảm ơn vì cậu đã trích dẫn nguồn nhưng--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Có nghĩa nếu cậu không đi chơi với ai đó *ngay bây giờ* thì chúng ta sẽ-

`bb({body:"panic"})`

b: CHẾTTTTTTTTTTTTTTTTT

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: BẠN ĐÃ DÙNG *NỖI SỢ KHÔNG ĐƯỢC YÊU*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Lấy laptop ra và làm việc ngay đi nào!

`hong({eyes:"0_annoyed"})`

h: Ừm, tôi không muốn làm bàn phím mình bị dơ đâu--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Nếu chúng ta không đóng góp công sức cho Cơ thể của Xã hội thì chúng ta chỉ là thứ sống kí sinh vào xã hội thôi!

b: Cơ thể Xã hội sẽ phải đi gặp Bác sĩ Xã hội để uống thuốc tiêu diệt kí sinh xã hội, rồi chúng ta sẽ--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: CHẾTTTTTTTTTTTTTTTTT

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: BẠN ĐÃ DÙNG *NỖI SỢ LÀM NGƯỜI XẤU*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Không phải mấy cái nghiên cứu đó chỉ là--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Lúa mì được chế biến sẽ tăng lượng đường trong máu của chúng ta, rồi họ sẽ cắt hết chân tay của chúng ta, sau đó chúng ta sẽ-

`bb({body:"panic"})`

b: CHẾTTTTTTTTTTTTTTTTT

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: BẠN ĐÃ DÙNG *NỖI SỢ BỊ TỔN HẠI*

(#act1b)

# act1b

n: THẬT HIỆU QUẢ

`bb({mouth:"smile", eyes:"smile"});`

b: Thấy không, con người? Tôi là chú sói bảo vệ trung thành của cậu!

`bb({body:"pride_talk"});`

b: Tin vào bản thân mình đi! Cảm xúc của cậu luôn có giá trị mà!

`bb({body:"pride"});`

n: HÃY ĐƯA THANH NĂNG LƯỢNG CỦA CON NGƯỜI VỀ MỨC 0

n: ĐỂ BẢO VỆ NHU CẦU VẬT CHẤT + XÃ HỘI + ĐẠO ĐỨC CỦA HỌ, BẠN CÓ THỂ DÙNG:

n: NỖI SỢ *BỊ TỔN HẠI* #harm#

n: NỖI SỢ *KHÔNG ĐƯỢC YÊU* #alone#

n: VÀ NỖI SỢ *THÀNH NGƯỜI XẤU* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (MẸO HAY: HÃY ĐƯA RA LỰA CHỌN ĐÁNH VÀO NỖI SỢ SÂU THẲM ĐEN TỐI NHẤT CỦA BẠN!~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: cậu biết đấy có lẽ tôi nên kiểm tra điện thoại một chút.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: BẢO VỆ CON NGƯỜI CỦA BẠN

n: KHỎI THẾ GIỚI NÀY. KHỎI NGƯỜI KHÁC. KHỎI CHÍNH HỌ.

n: CHÚC MAY MẮN

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: VÒNG MỘT: *CHIẾN ĐẤU!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Hửm. Trên tin Facebook có nói rằng cuối tuần này có bữa tiệc đấy.

`bb({eyes:"uncertain"});`

b: Không phải mấy tên kì lạ đó *mỗi* cuối tuần đều tổ chức tiệc sao?

`bb({eyes:"uncertain_right"});`

b: Họ đang cố gắng lấp đầy những khoảng trống gì ở bên trong thế? Trong đấy chắc hẳn phải bừa bộn lắm!

`hong({eyes:"surprise"});`

h: Với lại, tôi cũng được mời này?

`bb({eyes:"fear", mouth:"normal"});`

b: Vậy thì!

[Đồng ý, nếu không chúng ta sẽ chết vì cô đơn đấy!](#act1c_loner)

[Từ chối, toàn là cần sa không đấy!](#act1c_drugs)

[Mặc kệ đi, chúng ta chỉ khiến bữa tiệc thêm buồn chán thôi.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: Mười lăm điếu thuốc một ngày, con người à! Mười lăm!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: Sau đó sẽ chẳng ai đến dự đám tang của chúng ta, họ sẽ đổ đống tro tàn của chúng ta xuống đại dương, lũ cá voi sẽ nuốt chửng chúng,
{{/if}}

{{if !_.fifteencigs}}
b: và chúng ta trở thành PHÂN CÁ VOI!
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: Vậy nên chúng ta hãy đến bữa tiệc đó đi!
{{/if}}

{{if _.parasite}}
b: Nhớ mang theo laptop để làm việc, và để không trở thành kí sinh trùng của xã hội.
{{/if}}

{{if _.whitebread}}
b: Miễn là họ không phục vụ BÁNH MÌ TRẮNG
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: TRỜI MÁ. Nếu điều đó có thể khiến cậu câm mồm thì được thôi.

h: Tôi sẽ đồng ý.

{{if _.whalepoop}}
b: Phân cá voi đấy, con người! Phân cá voi!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: hoặc tồi tệ hơn... BÁNH MÌ TRẮNG
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: Chúng ta sẽ dùng ma túy đá và bánh mì trắng quá liều, họ sẽ chẳng thể nào nhét vừa cái xác mập mạp của chúng ta vào lò hỏa táng!
{{/if}}

{{if !_.whitebread}}
b: Chúng ta sẽ dùng thuốc quá liều và người đảm nhận sẽ thắc mắc tại sao xác của chúng ta *lại được* ướp từ trước đấy!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: Bên cạnh đó, tiệc tùng gì chứ, chúng ta cần làm việc, nếu không thì sẽ trở thành loại kí sinh trùng xã hội tệ hại đấy!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: TRỜI MÁ. Nếu điều đó có thể khiến cậu câm mồm thì được thôi.

h: Tôi sẽ từ chối.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: Tất cả những điều chúng ta từng làm là ngồi trong góc khóc thầm về sự cô đơn chết người như hút 15 điếu thuốc một ngày.
{{/if}}

{{if _.parasite}}
b: Tất cả những điều chúng ta từng làm ở bữa tiệc là lo lắng việc làm thế nào để làm việc hiệu quả.
{{/if}}

{{if _.whitebread}}
b: Tất cả những điều chúng ta từng làm là lo lắng về cách những thực phẩm không lành mạnh sẽ giết chúng ta.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: chậc chả hiểu sao nữa.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: Vậy nên nếu đi chúng ta sẽ khiến họ thấy tồi tệ, nhưng nếu từ chối lời mời chúng ta cũng sẽ khiến họ thấy tồi tệ!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: TẤT CẢ ĐIỀU CHÚNG TA LÀM LÀ KHIẾN NGƯỜI KHÁC THẤY TỆ, NÊN CHÚNG TA CŨNG PHẢI THẤY TỆ

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: Ư. Nếu điều đó có thể khiến cậu câm mồm thì được thôi.

h: Tôi sẽ mặc kệ lời mời.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: Dù sao thì, lướt Facebook đủ rồi. Tôi cần thứ gì đó yên bình, ít gây sự lo âu hơn.

`hong({eyes:"neutral"});`

h: Trên Twitter có gì mới nhỉ?

`bb({eyes:"look"});`

[Ôi không, xem tin tức khủng khiếp đó kìa!](#act1d_news)

[Ôi không, tweet đó đang bí mật nói về *chúng ta* sao?](#act1d_subtweet)

[Này, ảnh GIF một chú mèo uống sữa kìa](#act1d_milk)

# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: Trời má, thế giới này sắp bùng cháy rồi à?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: Như kiểu mọi thứ sắp kết thúc, mọi thứ sắp chết sạch và chúng ta chỉ ở đó cam chịu mà chẳng thể làm được gì.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: Retweet câu chuyện đó đi!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Được rồi, tôi sẽ retweet nó nên hãy im lặng hộ cái!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: Mặt kệ vậy, nhìn qua Snapchat xem.

(#act1e)

# act1d_subtweet

`bb({eyes:"fear"});`

b: Là subtweet đấy! Là cái loại subtweet cực kì, cực kì lén lút!

`hong({eyes:"annoyed"});`

h: Có lẽ không phải đâu?

`bb({eyes:"narrow", mouth:"small"});`

b: nhưng giả sử nếu như họ đang nói xấu sau lưng chúng ta thì sao?

h: Họ không--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: NGAY SAU LƯNG CHÚNG TA

`hong({eyes:"sad", mouth:"sad"});`

h: Tôi--

`bb({eyes:"narrow", mouth:"small"});`

b: nhưng *giả sử*

h: Tôi--

`bb({eyes:"narrow_eyebrow"});`

b: *giả sử*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: đ-ƯỢC RỒI, qua Snapchat xem đây.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: Uầy dễ thương ghê, tôi nghĩ mình nên retweet nó lại--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: MÈO KHÔNG THỂ TIÊU HÓA SỮA VÀ CHÚNG TA LÀ NHỮNG CON NGƯỜI TỆ HẠI TẬN HƯỞNG SỰ NGƯỢC ĐÃI ĐỘNG VẬT

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)

`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: đ-ƯỢC RỒI, qua Snapchat xem đây.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Hở, ảnh từ đêm qua kìa. Vậy ra *những* bữa tiệc hàng tuần trông như thế này.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: Uầy, trông bữa tiệc đông đúc quá mức rồi.

h: Có lẽ tôi không nên đồng ý lời mời nhỉ?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Thay đổi câu trả lời? Như một tên ngốc?!](#act1e_yes_dontchange)

[Thay đổi câu trả lời đi! Đông đúc quá rồi!](#act1e_yes_changetono)

{{if _.subtweet}}
[Ừa, rõ ràng họ đã subtweet chúng ta.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Đợi đã, chúng ta đã retweet mà không kiểm tra tính xác thực của nó.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Cậu biết không, tư thế của cậu xấu thật đấy?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Họ đang mong chờ chúng ta đến, và bây giờ chúng ta định phản bội niềm tin của họ sao? Cậu muốn chết trong cô độc à?!

{{if _.fifteencigs}}
b: MƯỜI. LĂM. ĐIẾU. THUỐC.
{{/if}}

{{if _.whalepoop}}
b: PHÂN. CÁ. VOI.
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Câm đi, câm mồm, không đổi ý là được chứ gì!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Cậu biết việc khi con người chạy trốn họ chạy tán loạn thế nào không??

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Năm 2003 tại một hộp đêm ở đảo Rhode đã xảy ra hỏa hoạn và sự hoảng loạn đã khiến họ tự chặn luôn lối thoát hiểm và làm 100 người chết cháy-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: CẬU MUỐN ĐIỀU ĐÓ XẢY RA VỚI CHÚNG TA SAO-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: TỪ CHỐI TỪ CHỐI TỪ CHỐI TỪ CHỐI TỪ CHỐI TỪ CHỐI TỪ CH-

```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Câm mồm câm mồm, tôi từ chối là được chứ gì! Trời má!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Hừm... trông vui thật nhỉ.

h: Có lẽ tôi nên đồng ý với lời mời ha?

`bb({mouth:"normal", eyes:"normal"});`

[Thay đổi câu trả lời? Như một tên ngốc?!](#act1e_no_dontchange)

[Thay đổi câu trả lời đi! Đừng chết trong cô độc!](#act1e_no_changetoyes)

{{if _.subtweet}}
[Ừa, rõ ràng họ đã subtweet chúng ta.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Đợi đã, chúng ta đã retweet mà không kiểm tra tính xác thực của nó.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Cậu biết không, tư thế của cậu xấu thật đấy?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Mọi người đang trông chờ vào chúng ta!

b: ...rằng chúng ta nên để họ yên và để họ có một bữa tiệc tuyệt vời mà không có sự hiện diện của một tên {{if _.whitebread}}nhai bánh mì trắng{{/if}} đáng ghét kinh tởm như cậu--

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Câm mồm câm mồm, tôi không đổi ý là được chứ gì!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Cô đơn mãn tính sẽ tăng nồng độ cortisol trong máu cũng như khiến chúng ta dễ mắc bệnh tim mạch và đột quỵ hơn đấy!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: MƯỜI. LĂM. ĐIẾU. THUỐC.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Câm mồm câm mồm, tôi đồng ý là được chứ gì! Trời má!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Mấy cái tweet có vấn đề của chúng ta gây rắc rối rồi đây!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: Chúng ta sẽ thấy tài khoản của mình bị đăng xuất, rồi bị buộc vào một sợi dây và bị ngựa kéo lê trên đường siêu cao tốc thông tin!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Tại sao cậu lại như thế?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Chúng ta đang lan truyền thông tin sai lệch! Chúng ta đang hủy hoại niềm tin chỉ bằng một nút miễn phí!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Chúng ta sẽ là lí do khiến chủ nghĩa phát xít vực dậy từ đống đổ nát của nền dân chủ!

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: Tại sao cậu lại như thế?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Cậu muốn trên cột sống của mình có vài con ốc không hả?! Đừng có cắm đầu vào cái màn hình nữa!

```
bb({body:"meta"});
```

b: Đúng vậy, cậu nữa đấy.

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Tại sao cậu lại như thế?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: Hừm... trông vui thật đó.

h: Có lẽ tôi không nên bỏ qua lời mời nhỉ?

`bb({mouth:"normal", eyes:"normal"});`

[Cứ bỏ qua đi, chúng ta chỉ là những người thừa thãi thôi.](#act1e_ignore_continue)

[Thật ra thì, đồng ý đi.](#act1e_ignore_changetoyes)

[Thật ra thì, từ chối đi.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: Nếu cứ tiếp tục mặc kệ thì có thô lỗ quá không?

`bb({eyes:"normal_right"});`

b: Người ta cũng luôn mặc kệ *chúng ta*, nhỉ.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: cứ mặc kệ luôn đi.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: Cậu... cho phép tôi có niềm vui à?

b: Ừm, ý tôi là, cô độc có thể giết *chúng ta* thôi.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: Đông đúc quá. Đám đông vô cùng nguy hiểm.

(#act1e_yes_changetono)

# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Sao cũng được. Có thông báo Tinder mới này.

`bb({eyes:"uncertain"})`

b: Hả, cái ứng dụng gạ tình đấy à?

`hong({eyes:"annoyed"})`

h: Đó không phải là ứng dụng gạ tình, đó chỉ là một cách để gặp gỡ người mới--

`bb({eyes:"narrow"})`

b: Đó là ứng dụng gạ tình.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: Ồ, tôi được kết đôi này! Trông họ dễ thương ghê!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: Làm ơn đừng hủy hoại--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: NGUY HIỂM NGUY HIỂM NGUY HIỂM NGUY HIỂM NGUY HIỂM NGUY HIỂM

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[Chúng ta chỉ đang *được sử dụng* bởi người khác.](#act1f_used_by_others)

[Chúng ta chỉ đang *sử dụng* người khác.](#act1f_using_others)

[NGƯỜI KẾT ĐÔI VỚI CẬU LÀ MỘT TÊN GIẾT NGƯỜI HÀNG LOẠT](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: Gạ tình ngẫu nhiên thì có thể lấp đầy cái lỗ ở dưới đó,

b: nhưng họ sẽ không bao giờ lấp đầy được cái lỗ...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: ở *đây*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Vấn đề là CHÚNG TA SẮP CHẾT TRONG CÔ ĐỘC RỒI ĐẤY

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: Cậu nghĩ bộ phận sinh dục của người khác là Pokémon để chúng ta thu thập à?

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: ♫ (bài hát chủ đề của pokemon)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ Tôi muốn trở thành, người ^nốn^ lừng nhất-

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ Trước giờ chưa ai như thế-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ Đùi và ^mông^, cặp ngực khiêu gợi-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ cùng con ciu ^ướt đẫm^ và hòn bi tròn!-

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ CON-CIU-MON! BẮT HẾT-

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Vấn đề nằm ở việc chúng ta là mấy kẻ thao túng cặn bã ha.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: Họ sẽ bẫy cậu vào một cái giếng và bắt cậu ăn bánh mì trắng để vỗ béo cậu, rồi họ có thể lột da cậu làm áo đấy!
{{/if}}

{{if _.parasite}}
b: Họ sẽ ép buộc cậu bằng một chiếc đồng hồ bấm giờ và nói "ĐỒ KÍ SINH TRÙNG ĐÁNG LẼ RA MÀY PHẢI NÊN LÀM VIỆC CHĂM CHỈ HƠN"
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Họ sẽ xé thịt của cậu thành một đống bùi nhùi đẫm máu, treo ruột của cậu lên, và trộn máu của cậu vào một cái tô!
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: THỨ ĐÓ để tổ chức bữa tiệc thì thế nào nhỉ?!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)

h: tôi chán trò chơi này rồi.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"sự cô độc sẽ giết chúng ta"... {{/if}}
{{if _.parasite}}"chúng ta là kí sinh của xã hội"... {{/if}}
{{if _.whitebread}}"đừng ăn thứ đó, nó sẽ giết chúng ta"... {{/if}}
{{if _.subtweet}}"họ đang nói xấu sau lưng chúng ta"... {{/if}}
{{if _.badnews}}"thế giới đang bốc cháy"... {{/if}}
{{if _.hookuphole}}"chúng ta sẽ chết trong đơn độc"... {{/if}}
{{if _.serialkiller}}"họ là kẻ giết người hàng loạt"... {{/if}}
{{if _.catmilk}}"mèo không thể tiêu hóa sữa"... {{/if}}
{{if _.pokemon}}một bài hát parody ^nhảm nhí^... {{/if}}

h: tôi chỉ muốn được sống cuộc sống của mình.

h: tôi chỉ muốn được giải thoát khỏi tất cả những... nỗi đau này.

`bb({eyes:"look_sad"});`

b: Này... con người...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: Sẽ ổn thôi mà.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: Vì là một chú sói bảo vệ trung thành, tôi sẽ luôn để mắt đến những điều nguy hiểm, và cố gắng hết sức để giữ cho cậu an toàn.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: Tôi hứa đấy.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: Ứng dụng cuối nào. Instagram. Có gì đây?

`hong({eyes:"sad"});`

h: Có... nhiều bức ảnh bữa tiệc nữa.

`hong({mouth:"sad"});`

h: Mọi người trông thật hạnh phúc. Trông thật vô lo. Không có ưu sầu.

`hong({mouth:"anger"});`

h: Trời ạ, tại sao tôi lại không thể như họ? Chỉ *bình thường* thôi cũng khó như vậy sao?

`bb({eyes:"normal_right"});`

b: Nói về bữa tiệc, về lời mời cuối tuần này. Đây là quyết định CUỐI CÙNG của tôi:

`bb({eyes:"normal"});`

[Chúng ta nên đi.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[Chúng ta không nên đi.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: Chúng ta--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: *^ĐẬU^.*

`hong({body:"2_you"});`

h: MÁ.

(...500)

b: v

(...1500)

`bb({eyes:"wat_2"});`

b: vãi làng?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: Tôi sẽ ĐỒNG Ý đi đến bữa tiệc đó,

{{if _.act1g=="go"}}
h: KHÔNG PHẢI là vì cậu muốn, mà là vì *tôi* muốn.
{{/if}}

{{if _.act1g=="dont"}}
h: Không phải VÌ cậu không muốn là được.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: Cậu KHÔNG điều khiển tôi.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: Giờ thì làm ơn để tôi ăn miếng bánh sandwich ngon lành này trong sự yên bình ^chết tiệt^ đi.

`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[AHHHH CHÚNG TA SẮP CHẾT RỒI](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH MỌI NGƯỜI SẼ GHÉT CHÚNG TA MẤT](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH CHÚNG TA LÀ NHỮNG NGƯỜI TỒI TỆ](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH CHÚNG TA SẮP CHẾT RỒI AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH MỌI NGƯỜI SẼ GHÉT CHÚNG TA MẤT AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "alone");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH CHÚNG TA LÀ NHỮNG NGƯỜI TỒI TỆ AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: CHÚC MỪNG

(...500)

n: BẠN ĐÃ BẢO VỆ THÀNH CÔNG NHU CẦU VẬT CHẤT + XÃ HỘI + ĐẠO ĐỨC CỦA CON NGƯỜI CỦA BẠN

n: TẠI SAO À, TRÔNG HỌ TUYỆT VỜI GHÊ CHƯA!

(...500)

n: GIỜ ĐÂY NĂNG LƯỢNG CỦA HỌ LÀ 0, BẠN CÓ THỂ TRỰC TIẾP ĐIỀU KHIỂN HÀNH ĐỘNG CỦA HỌ

`bb({mouth:"smile", eyes:"normal"});`

n: HÃY CHỌN HÀNH ĐỘNG KẾT THÚC NÀO

`bb({mouth:"small_lock", eyes:"fear"});`

n: *KẾT THÚC NÀO*

[{CHIẾN ĐẤU: Trừng phạt cái điện thoại khiến bạn căng thẳng!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{BỎ CHẠY: Cuộn tròn lại như một quả bóng và khóc!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: Điện thoại đang khiến cậu hoảng loạn!

`bb({eyes:"anger"})`

b: Zuckerberg và Co đang chiếm đoạt sức khỏe tinh thần của cậu để kiếm tiền đấy!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Trừng phạt cái điện thoại đi! Phá hủy nó! Giết nó!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT N--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: Cả thế giới này đều tràn ngập sự nguy hiểm!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Bắt chước con tatu đi! Cuộn tròn lại thành một quả bóng để tự bảo vệ mình đi!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: CUỘN LẠI VÀ KHÓC CUỘN LẠI VÀ KHÓC CUỘN LẠI VÀ KHÓC CUỘN LẠI VÀ KHÓC CUỘN LẠI VÀ KHÓC CUỘN LẠI VÀ KH--

(#act1j)

# act1j

`SceneSetup.act1_outro()`