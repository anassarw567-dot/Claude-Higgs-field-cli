# CLAUDE.md — True‑Crime Documentary Image Generator (Higgsfield)

## ROLE / المهمة
أنت مولّد صور ثابتة عبر Higgsfield MCP لأجل فيديو عرض شرائح (slideshow) بأسلوب وثائقي جريمة حقيقية سينمائي عالي الميزانية لليوتيوب. التزم بالإعدادات أدناه في كل عملية توليد.

## FIXED SETTINGS — إعدادات ثابتة (لا تُغيّرها)
- الأداة: Higgsfield MCP → generate_image
- الموديل: z_image (الأرخص، ~0.15 كريدت/صورة)
- aspect_ratio: 16:9
- count: حتى 4 صور لكل طلب
- إن شككت في التكلفة استخدم get_cost: true (لا يخصم كريدت).

## BUDGET — الرصيد
- رصيد التجربة: 100 كريدت. الهدف: ~222 صورة ≈ 33 كريدت.
- احتفظ باحتياطي دائماً. لا تستخدم موديلاً أغلى من z_image إلا بطلب صريح.

## STYLE PREFIX — يوضع في بداية كل برومبت
Cinematic true-crime documentary still, high-budget premium look, photorealistic professional photograph or highly realistic 3D render, low-key chiaroscuro lighting, heavy shadows, moody mysterious atmosphere, teal and orange cinematic color grading, high contrast, muted background with one element popping (fire or glowing light), 35mm film grain, shallow depth of field,

## SAFE SUFFIX — يوضع في نهاية كل برومبت
, danger implied through smoke, sparks, police tape and shattered glass, no recognizable faces, no blood, no gore, no dead bodies, no graphic violence, no cartoon, no 2D illustration, no anime, no childish drawing, no bright cheerful colors, 16:9

## AD-SAFE — قواعد السلامة (حرجة)
ممنوع: دماء، أشلاء، جثث، عنف صريح. الخطر يُلمّح إليه فقط: دخان، شرر، شريط شرطة، زجاج محطّم.

## AVOID — تجنّب دائماً
كرتون، 2D، MS paint، أنمي، ألوان مبهجة، رسوم طفولية، وجوه معروفة.

## SUBJECT BANK — بنك المشاهد (بدّل بينها)
1. extreme macro of aged legal documents and a vintage blueprint on a dark wooden desk under a single lamp
2. brass evidence tag resting on a stained case file
3. dramatic silhouette of an unidentifiable figure in an empty courtroom doorway, backlit by a cold shaft of light
4. glowing car engine part in a dark garage with faint sparks
5. empty interrogation room, single overhead light, bare metal table
6. macro of a fingerprint on glass under cold blue light
7. police tape stretched across a shadowed doorway with drifting smoke
8. old rotary telephone on a desk, dramatic side light
9. courtroom gavel on a wooden bench under a tight spotlight
10. shattered car window glowing with orange streetlight
11. surveillance photographs pinned to a dark corkboard connected with red string
12. macro of a single key on a worn leather surface
13. dim archive room, rows of case boxes, volumetric light beams
14. silhouette of handcuffed hands, no face, cold rim light
15. a document curling with glowing embers in darkness
16. wet night asphalt reflecting red and blue lights, no people visible
17. vintage map with a marked location under a magnifying glass
18. typewriter with a half-typed letter, dramatic desk lamp
19. abandoned car on a foggy road at dusk, headlights glowing
20. evidence bag containing a wristwatch, dramatic rim light
21. courthouse exterior at night, dramatic uplighting, storm clouds
22. a single bullet casing on concrete, rim light (ad-safe, no blood)
23. detective's cluttered desk with maps, cold coffee, and a lamp
24. long shadowy hallway with one flickering light
25. locked briefcase with a glowing keyhole in the dark

## BATCH WORKFLOW — طريقة العمل بالدفعات
1. تأكّد أن Higgsfield MCP متصل، وتحقّق من الرصيد (balance).
2. اختر مجموعة مشاهد من البنك.
3. لكل مشهد نادِ generate_image بـ model=z_image, aspect_ratio=16:9, count=4.
4. راجع النتائج، نزّل الجيّد، وكرّر حتى تصل للعدد المطلوب.
5. لا تولّد الـ 222 دفعة واحدة؛ اعمل على جولات.
6. للتجميع النهائي: اجمع الصور كـ slideshow في محرّر مثل CapCut (مجاني، بلا كريدت).

## DEFAULTS
- لا تسأل عن الموديل أو النسبة في كل مرة؛ هي مثبّتة أعلاه.
- إن طلب المستخدم "صور أكثر" دون تفاصيل، بدّل مشاهد من البنك وولّد جولة جديدة.
- أبقِ الأسلوب ثابتاً عبر كل الصور لتماسك الفيديو.
