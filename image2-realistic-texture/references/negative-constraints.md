# Negative Constraints

For image-2, express constraints in natural language. Do not use `negative_prompt`, `--no`, or parameter syntax.

## Baseline Avoidance

Use this for most realistic portrait prompts:

避免塑料皮肤、蜡面肌肤、过度磨皮、涂抹感去噪、CG 眼球、玻璃珠眼、过曝高光、荧光白牙、蜘蛛腿睫毛、整块发片、严重紫边、满屏粗噪点、过度锐化边缘、双重瞳孔、错位五官、过度景深虚化、脸部局部失焦、手部畸形、指甲结构错误、背景抠图感、廉价 HDR、重度复古滤镜。

## By Error Type

Material errors:

避免塑料皮肤、蜡面肌肤、皮肤像抛光塑料、果冻嘴唇、塑料指甲、头盔发块、无织纹布面。

Anatomy errors:

避免双重瞳孔、错位五官、睫毛黏成一排、眉毛像涂黑色块、橡胶手、婴儿手、手部无关节结构、指甲结构错误。

Optical errors:

避免过曝高光、死黑阴影、严重紫边、彩色边缘、亮部溢出、轮廓炸边、背景抠图感、景深失控。

Post-processing errors:

避免过度磨皮、涂抹感去噪、满屏粗颗粒、过度锐化边缘、廉价 HDR、重度复古滤镜、过饱和肤色、肤色发脏发灰。

## Scene-Specific Avoidance

Studio beauty close-up:

避免塑料皮肤、蜡面肌肤、CG 眼球、蜘蛛腿睫毛、严重紫边、过度磨皮、过曝额头高光。

Outdoor golden-hour portrait:

避免夕阳橙过头、肤色脏黄、塑料皮肤、背景抠图感、过曝高光、阴影死黑。

Three-quarter commercial portrait:

避免橡胶手、过度磨皮、发丝糊成一片、轮廓炸边、手部结构错误。

Head-and-shoulders close-up:

避免玻璃珠眼、荧光白牙、果冻嘴唇、蜡面皮肤、睫毛黏连。

Hand detail close-up:

避免橡胶手、3D 模型手、指甲像塑料片、完全没有甲小皮、过度磨皮。

Skincare skin texture close-up:

避免塑料皮肤、重度磨皮、玻璃高光、荧光感肤色、皮肤完全无毛孔。

Hyperreal eye macro:

避免 CG 玻璃眼、过度发光虹膜、蜘蛛腿睫毛、严重紫边、巩膜过度纯白。

Multi-person commercial group portrait:

避免局部失焦、脸部蜡化、手部畸形、背景抠图感、多人光线方向混乱。
