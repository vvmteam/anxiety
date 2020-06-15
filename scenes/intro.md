# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

```
_.PLAYED_BEFORE = !!window.localStorage.continueChapter;
```

{{if !_.PLAYED_BEFORE}}
`Game.OVERRIDE_FONT_SIZE=30;`
{{/if}}

{{if !_.PLAYED_BEFORE}}
[#play1# CHƠI! #play2#](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="act2"}}
[_TIẾP TỤC_: Bữa tiệc](#act2) `publish("LOAD_GAME", ["act2"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="act3"}}
[_TIẾP TỤC_: Bữa tiệc khác](#act3) `publish("LOAD_GAME", ["act3"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="act4"}}
[_TIẾP TỤC_: Bánh Sandwich khác](#act4) `publish("LOAD_GAME", ["act4"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="replay"}}
`Game.OVERRIDE_FONT_SIZE=30;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="replay"}}
[#play1# CHƠI LẠI! #play2#](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE}}
[Chọn chương](#chapter-select) `Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

[(nội dung ghi chú)](#intro-play-button) `Game.OVERRIDE_CHOICE_LINE=true; publish('show_cn');`

# chapter-select

`publish("HACK_chselect");`

[I. Bánh Sandwich](#intro-start) `publish("HACK_chselect_end"); publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

[II. Bữa tiệc](#act2) `publish("HACK_chselect_end"); publish("LOAD_GAME", ["act2"]); Game.OVERRIDE_CHOICE_LINE=true;`

{{if window.localStorage.act3}}
[III. Bữa tiệc khác](#act3) `publish("HACK_chselect_end"); publish("LOAD_GAME", ["act3"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if !window.localStorage.act3}}
[III. Bữa tiệc khác]()
{{/if}}

{{if window.localStorage.act4}}
[IV. Bánh Sandwich khác](#act4) `publish("HACK_chselect_end"); publish("LOAD_GAME", ["act4"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if !window.localStorage.act4}}
[III. Bánh Sandwich khác]()
{{/if}}

{{if window.localStorage.credits}}
[V. Thông tin](#to-credits) `publish("HACK_chselect_end"); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if !window.localStorage.credits}}
[V. Thông tin]()
{{/if}}

[(menu chính)](#intro-play-button) `publish("HACK_chselect_end"); Game.OVERRIDE_CHOICE_LINE=true;`

# to-credits

`stopAllSounds();`

(...101)

(#credits)

# intro-start

(...500)

`clearText()`

n3: Xin chào! Đây không giống một "trò chơi" lắm, giống một câu chuyện tương tác hơn. Hy vọng bạn sẽ thích nhé!

n3: Vậy trước khi chúng ta bắt đầu, *bạn* muốn đọc thế nào?

`publish("show_options_bottom")`

# intro-start-2

n3: Tuyệt lắm! Lưu ý: bạn luôn có thể thay đổi cài đặt bằng icon ⚙ ở bên dưới. Thêm nữa, trò chơi sẽ tự động lưu ở mỗi chương!

n3: Nào, hãy bắt đầu câu chuyện của chúng ta thôi...

`clearText()`

(...1000)

`publish("intro-to-game-2")`

n2: ĐÂY LÀ MỘT CON NGƯỜI

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`