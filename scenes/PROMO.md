# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[CHƠI!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Vậy trước khi chúng ta bắt đầu, *bạn* muốn đọc thế nào?

`publish("show_options_bottom")`

# intro-start-2

n3: Nào, hãy bắt đầu câu chuyện thôi...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: ĐÂY LÀ MỘT CON NGƯỜI

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: VÀ ĐÂY LÀ SỰ LO ÂU CỦA CON NGƯỜI

n: _BẠN_ LÀ SỰ LO ÂU ĐẤY

(#act1_normal)

# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Nầu. Không, không, không nghe gì hết. Kiểm tra điện thoại thôi.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: CÔNG VIỆC CỦA BẠN LÀ BẢO VỆ CON NGƯỜI CỦA BẠN KHỎI *SỰ NGUY HIỂM*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Uầy! Cậu đang quăng cuộc sống của mình lên Twitter! Lại nữa!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h:Ừa, tôi đang tự hỏi tại sao tôi lại không ngồi xuống và lắng nghe suy nghĩ của mình thường xuyên hơn.

`hong({eyes:"neutral"});`

n: NHANH LÊN, CẢNH BÁO HỌ VỀ *SỰ NGUY HIỂM!*

```
bb({eyes:"look"});
```

[Ôi không, xem tin tức khủng khiếp đó kìa!](#act1d_news)

[Ôi không, tweet đó đang bí mật nói về *chúng ta* sao?](#act1d_subtweet)

[Này, ảnh GIF một chú mèo uống sữa kìa](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Ầy dễ thương phết, tôi--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: MÈO KHÔNG THỂ TIÊU HÓA SỮA VÀ CHÚNG TA LÀ NHỮNG CON NGƯỜI TỆ HẠI TẬN HƯỞNG SỰ NGƯỢC ĐÃI ĐỘNG VẬT

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```
