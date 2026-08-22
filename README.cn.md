# 猫爪测试点及治具

中文说明 | [English](README.md)

本仓库包含了“猫爪”形状的测试点设计文件，包括 KiCad 封装和治具设计与生产文件。

![footprint](https://user-images.githubusercontent.com/8038511/173807471-f3634d36-5d1a-4202-bad3-2db55b7f6b24.png)

## KiCad 封装
在 `Local.pretty` 文件夹中，有两种类型的 KiCad 封装。

 * 如果你不需要过孔，你可以使用 `meow.kicad_mod`。这是一个没有过孔的单面封装。
 * 如果你需要双面连接或者多层板，`meow_hole.kicad_mod` 在猫爪的“爪尖”处包含过孔，过孔可以让你的“猫爪”更加美观。

所有封装的 Edge Cuts 层都包含了定位孔。

## 治具
本仓库也包含了猫爪测试点的治具。它们都需要探针来进行组装。

我们建议使用针管直径为 1.0mm 的探针，并且强烈建议使用分体式的探针，例如 P50 系列。因为高温会损坏一体式的探针。

我们强烈建议使用圆头探针，因为尖头探针可能会损伤猫爪的焊盘的美观性。

你还需要两个直径为 1.0mm、长度为 16mm 的定位销。

有两种类型的治具。

### 测试探针治具
测试探针治具是一种手持式的测试工具。这种治具非常适合用于批量烧录芯片。

你可以在 `TestNeedle` 文件夹中找到其 PCB 设计文件。

![Needle](https://user-images.githubusercontent.com/8038511/173817801-1c8001b9-4a99-4336-ba42-3ec8435dd885.png)

![Needle2](https://user-images.githubusercontent.com/8038511/173817502-b0202656-4881-4886-84db-a64d9fba86ee.png)

### 夹子治具
夹子治具是一种稳定连接到 PCB 的好方法，非常适合用于芯片调试。`Clip` 文件夹包含了一个 FreeCAD 设计文件 `Fixture.FCStd`，你可以使用 PETG 或其他坚固的 3D 打印材料来打印它。配套的转接 PCB 设计也包含在 `Clip` 文件夹中。

你需要使用三个 M2 * 12mm 螺丝来组装这个治具，其中两个用于固定夹子主体和转接 PCB，一个用于组装夹子部件。

这种类型的治具需要一个线径 0.7mm * 外径 7mm * 长度 20mm 的弹簧来配合使用。

![Clip](https://user-images.githubusercontent.com/8038511/173806358-feefa180-b81d-44e4-99a9-08597d6d76a1.png)

![Clip2](https://user-images.githubusercontent.com/8038511/173818526-0935264e-4586-4c19-85a8-690d3c33e9f0.png)
