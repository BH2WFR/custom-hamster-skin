# 个人使用 iOS Hamster 输入法主题



基于 **咖啡** 提供的 **极简·蓝** 修改





## 外观:

<img src="./assets/image-20251116205621035.png" alt="image-20251116205621035" style="zoom:50%;" />

<img src="./assets/122ee5f3816a9d7912bf1c9108f9f050.png" alt="122ee5f3816a9d7912bf1c9108f9f050" style="zoom: 50%;" />

<img src="./assets/image-20251116205645869.png" alt="image-20251116205645869" style="zoom:50%;" />

<img src="./assets/image-20251116205654212.png" alt="image-20251116205654212" style="zoom:50%;" />





# 使用说明：

## 主题文件

在 `/custom-1` 文件夹中，分亮、暗两个主题；横屏、竖屏、浮动键盘三种模式。

**目前仅在 iPad 上测试，iPhone 上的效果未知。**



## 针对全拼用户

如果使用的是全拼输入法，请将 `pinyin_26_**.yaml` 文件中

```yaml
shiftButton:
  size:
    width:
      percentage: 0.15
    height:
      percentage: 1
  bounds:
    width: 95/100
    height:
      percentage: 1
    alignment: left
  backgroundStyle: shiftButtonBackgroundStyle
  foregroundStyle:
    - shiftButtonForegroundStyle
    - shiftButtonUpForegroundStyle
    - shiftButtonDownForegroundStyle
  uppercasedStateForegroundStyle: shiftButtonUppercasedForegroundStyle
  capsLockedStateForegroundStyle: shiftButtonCapsLockedForegroundStyle
  preeditStateForegroundStyle: shiftButtonPreeditStateForegroundStyle
  hintStyle: shiftButtonHintStyle
  action: shift
  swipeUpAction: tab
  swipeDownAction: {shortcutCommand: '#capsLocked'}
  preeditStateAction: {character: ';'} # 微软双拼中的分号；如果是全拼，可以改成 `'` 分词符
```

把 ` preeditStateAction: {character: ';'}` 改为 ` preeditStateAction: {character: "'"}`

即可在输入过程中按 shift 键当分词符 `'` 键





'