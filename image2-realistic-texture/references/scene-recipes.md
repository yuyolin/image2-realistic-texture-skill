# Scene Recipes

Read this file before assembling a prompt. Match the user's request to the closest recipe, then use `module-library.md` for exact wording.

## Studio Beauty Close-Up

Triggers: 棚拍美容近景, 美妆近景, 高端棚拍, beauty close-up, studio beauty, 肤质近景.

Use:

- Subject/framing: 面部近景肖像，双眼清晰对焦.
- Modules: `SKN-01`, `EYE-01`, `HAR-01`, `LGT-01`, `LGT-02`, `LGT-03`, `CAM-01`, `IMG-01`, `POST-01`, `POST-02`.
- Avoid: plastic/waxy skin, CG eyes, spider-leg lashes, severe fringing, heavy smoothing.

Prompt base:

面部近景肖像，双眼清晰对焦，真实皮肤质感，清晰但克制的毛孔，皮肤微纹理可见，轻微次表面散射，局部受控镜面高光，轻微自然油脂光泽，眼表面轻微湿润，虹膜放射状纹理清晰，睫毛根根分明，眉毛毛流自然，发丝边缘有少量飞丝，大型柔光箱主光，白色 beauty dish 辅助塑形，细窄轮廓光勾边，中画幅成像感，105mm 镜头视角，f/5.6，低噪点，高光与阴影层次完整，克制的商业调色，轻微 dodge and burn，仅限轻度频率分离式修饰

## Outdoor Golden-Hour Portrait

Triggers: 户外黄金时刻, 夕阳人像, 自然光半身, golden hour portrait.

Use:

- Subject/framing: 半身近景肖像 or user-specified outdoor portrait.
- Modules: `SKN-01`, `SKN-02`, `EYE-01`, `HAR-02`, `LGT-05`, `CAM-02`, `IMG-01`, `IMG-02`, `POST-01`.
- Avoid: orange cast, overexposed highlights, cutout background, plastic skin.

Prompt base:

半身近景肖像，真实皮肤质感，毛孔与皮肤微纹理自然可见，肤色通透，少量自然雀斑可见，细小表情纹保留，眼表面轻微湿润，虹膜与睫毛清晰，发丝边缘有自然透光，黄金时刻低角度暖光，侧逆光，光线柔和，肤色温暖但不偏橙，背景柔和焦外，主体与背景分离明确，85mm 镜头视角，f/2.8，宽广动态范围，高光不过曝，阴影里仍保留纹理，轻微商业调色，极轻微胶片颗粒

## Three-Quarter Commercial Portrait

Triggers: 三分之四身, 商业人像, 半身偏全身, 人物带手, commercial portrait.

Use:

- Subject/framing: 三分之四身人物构图，脸部与手部都清楚.
- Modules: `SKN-01`, `HND-01`, `EYE-01`, `HAR-01`, `LGT-01`, `LGT-03`, `CAM-03`, `IMG-01`, `POST-01`.
- Avoid: rubber hands, over-smoothing, hair merged into blocks, blown rim light.

Prompt base:

三分之四身人物构图，脸部与手部都保持真实皮肤纹理，毛孔清晰但不过度夸张，手背皮肤纹理自然，关节轻微褶皱清楚，指甲边缘干净，甲小皮自然完整，眼表面轻微湿润，睫毛与眉毛方向自然，发丝分束清晰，大型柔光箱主光，侧后方细窄轮廓光，主体从背景中干净分离，中画幅成像感，90mm 镜头视角，f/4，低噪点，层次丰富，克制的商业调色，轻微 dodge and burn

## Head-And-Shoulders Close-Up

Triggers: 头肩特写, 大特写, 肖像特写, close-up portrait.

Use:

- Subject/framing: 头肩大特写，双眼准确对焦.
- Modules: `SKN-01`, `EYE-01`, `LIP-01`, `HAR-01`, `LGT-02`, `LGT-03`, `CAM-01`, `IMG-01`, `POST-02`.
- Avoid: glassy eyes, fluorescent teeth, jelly lips, waxy skin.

Prompt base:

头肩大特写，双眼准确对焦，真实毛孔与皮肤微纹理，轻微次表面散射，局部镜面高光受控，眼表面轻微湿润，虹膜纹理清楚，睫毛根根分明，眉毛毛流自然，唇纹清晰，唇面自然微干润，发丝分束自然，白色 beauty dish 主光，轻微补光控制阴影，细窄轮廓光勾边，105mm 镜头视角，f/5.6，宽容动态范围，色彩克制，低噪点，轻微商业调色，仅限轻度频率分离式修饰

## Hand Detail Close-Up

Triggers: 手部特写, 手部细节, 指甲, hand close-up.

Use:

- Subject/framing: 手部细节特写.
- Modules: `HND-01`, `LGT-04`, `LGT-03`, `CAM-04`, `IMG-02`, `POST-01`.
- Avoid: rubber hands, 3D model hands, plastic nails, over-smoothed skin.

Prompt base:

手部细节特写，手背皮肤纹理自然，关节结构与轻微褶皱清晰，指甲表面真实反光，甲缘干净，甲小皮自然完整，肤面光泽克制，纹理真实不粗糙，柔和侧光塑形，细窄轮廓光轻微勾边，100mm 微距镜头视角，f/8，低噪点，背景柔和焦外，轻微胶片颗粒，克制调色

## Skincare Skin Texture Close-Up

Triggers: 护肤品式皮肤特写, 皮肤质感特写, 毛孔特写, skincare close-up.

Use:

- Subject/framing: 面部皮肤质感特写.
- Modules: `SKN-03`, `EYE-01` if eyes are visible, `LIP-01` if lips are visible, `LGT-01`, `LGT-02`, `CAM-01`, `IMG-01`, `POST-01`, `POST-02`.
- Avoid: plastic skin, heavy smoothing, glass highlights, fluorescent skin tone.

Prompt base:

面部皮肤质感特写，真实而干净的毛孔，皮肤微纹理均匀，轻微次表面散射让肤色透气，局部细小镜面高光，轻微自然油脂光泽，仅 T 区有微弱光泽，肤色中性准确，细小表情纹保留，眼表面轻微湿润，唇纹自然，柔和大型主光，白色 beauty dish 轻微塑形，中画幅成像感，110mm 镜头视角，f/5.6，低噪点，高光与阴影层次完整，克制商业调色，轻微 dodge and burn，仅限轻度频率分离式修饰

## Hyperreal Eye Macro

Triggers: 眼部微距, 眼睛特写, 虹膜, 超写实眼部, eye macro.

Use:

- Subject/framing: 眼部超近景微距.
- Modules: `EYE-02`, `CAM-05`, `IMG-03`, `POST-01`.
- Avoid: CG glass eye, glowing iris, spider-leg lashes, severe fringing.

Prompt base:

眼部超近景微距，虹膜放射状纹理与色彩层次清晰，瞳孔边缘干净，眼表面轻微湿润，泪膜反光自然，巩膜真实不过度纯白，睫毛根根分明并有方向变化，眉毛短毛细节清楚，110mm 微距镜头视角，f/11，低噪点，高光控制准确，几乎无色差，极轻微辉光，背景完全柔和虚化，克制调色

## Multi-Person Commercial Group Portrait

Triggers: 多人群像, 商业群像, 团队照, group portrait, 多人同框.

Use:

- Subject/framing: 多人同框群像，所有人物关键面部结构清晰.
- Modules: `SKN-01`, `EYE-01`, `HAR-01`, `HND-01`, `LGT-01`, `LGT-03`, `CAM-06`, `IMG-01`, `IMG-02`, `POST-03`.
- Avoid: local face blur, waxy faces, malformed hands, cutout background.

Prompt base:

多人同框群像，所有人物双眼与关键面部结构清晰，真实皮肤质感，毛孔与皮肤微纹理自然可见，不做重度磨皮，眼表面轻微湿润，虹膜与睫毛清楚，发丝分束自然，手部结构与指甲细节真实，大型柔光箱主光统一照明，轻微补光保持阴影层次，细窄轮廓光帮助人物与背景分离，80mm 镜头视角，f/8，宽广动态范围，低噪点，色彩克制统一，极轻微胶片颗粒

## Fallback Recipe

Use this when the scene is a realistic portrait but does not match a named family:

用户给定主体与构图，真实皮肤质感，毛孔与皮肤微纹理自然可见，轻微次表面散射，局部受控镜面高光，眼表面轻微湿润，虹膜纹理自然，发丝分束清晰，光线柔和且方向明确，主体与背景分离自然，中画幅成像感，低噪点，高光与阴影层次完整，克制的商业调色，轻微 dodge and burn，仅限轻度保留纹理的修饰
