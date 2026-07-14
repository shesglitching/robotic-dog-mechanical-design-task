# استلهام التصميم من كلب الغريهاوند  
عندما قرأت أن المشروع عن تصميم كلب روبوتي، أول جملة خطرت ببالي – المعذرة – كانت:  
**"كل السلق اللي بالشعيب يطلعون."**

ولمن لا يعرف، فإن **كلب الغريهاوند (Greyhound)** ينتمي إلى نفس فئة **كلاب الصيد بالنظر (Sighthounds)** التي ينتمي إليها السلوقي، لكنه سلالة مختلفة. ويتميز ببنية جسدية فريدة؛ فهو من أسرع سلالات الكلاب وأكثرها كفاءة في الجري، إذ تصل سرعته إلى حوالي **72 كم/ساعة**. يمتلك تسارعًا عاليًا، وبنية رياضية، وجسمًا انسيابيًا يشبه الصاروخ، إضافة إلى هيكل مرن ووسائد أقدام سميكة توازن بين الحماية وخفة الحركة، كما تساعد على امتصاص الصدمات.

ويتميز أيضًا بـ:
- هيكل نحيف وانسيابي يقلل مقاومة الهواء (ديناميكية هوائية أفضل).
- بطن ضامر جدًا يساعد على خفة الحركة.
- جسم متناسق مصمم للسرعة والكفاءة.

لهذا استلهمت البنية الأساسية لكلبي الروبوتي من **الغريهاوند**، مع المحافظة على أهم خصائصه الجسدية، وذلك من خلال:

- بطن ضامر.
- صدر أعرض من البطن مع انحناء بسيط.
- ظهر منحني للخارج على شكل قوس.
- فخذ أعرض في البداية والنهاية وأنحف في المنتصف.
- ساق تكون أعرض من الأعلى وتضيق تدريجيًا باتجاه القدم.
- قدم دائرية مستوحاة من شكل أقدام الغريهاوند.
- استخدام مادة **TPU** لتغطية القدم، لما تتميز به من مرونة وقدرة على امتصاص الصدمات.
- إضافة أربع وسادات في الجزء الملامس للأرض، أيضًا من **TPU**، لمحاكاة وسائد أقدام الغريهاوند والمساعدة في تحسين الثبات وتقليل تأثير الصدمات أثناء الحركة.

## Initial Concept Sketch

<img width="966" height="821" alt="Initial Concept Sketch" src="https://github.com/user-attachments/assets/2e6a0e6a-600c-45bd-87b7-c6391cde498e" />

## Leg and Foot Design

- إضافة طبقة حماية مرنة من مادة **TPU** على منطقتي الظهر والبطن لتقليل الأضرار الناتجة عن السقوط أو الانقلاب أو الجلوس، مع توفير حماية إضافية للهيكل الخارجي للروبوت.

<img width="720" height="610" alt="Leg and Foot Design" src="https://github.com/user-attachments/assets/d53f7f3c-65c6-41d0-99e3-894fa3b4efa9" />

- تصميم مقدمة الجسم بحيث يتناقص عرضها كلما اتجهنا للأمام، وكذلك مؤخرة الجسم، لمحاكاة البنية الانسيابية الشبيهة بالصاروخ الموجودة في الغريهاوند.
- إضافة **حساس موجات فوق صوتية (Ultrasonic Sensor)** في مقدمة الجسم لتجنب الاصطدام بالعوائق والأجسام المحيطة.

## TPU Protective Layer and Sensor Design

<img width="817" height="658" alt="TPU Protective Layer and Sensor Design" src="https://github.com/user-attachments/assets/ac70e2c6-5317-4525-8e7a-93f91d6198bf" />

تساهم بنية الغريهاوند في تحقيق كفاءة عالية من خلال الاستفادة من خصائصه الميكانيكية، مع الحفاظ على تصميم عملي وقابل للتنفيذ. حيث يساعد هذا الشكل على **تقليل التكلفة، وتسهيل عملية التصنيع، وتحقيق موثوقية وكفاءة أعلى للهيكل**، وذلك بسبب بساطة المكونات وتقليل التعقيد في التصميم.

---

# Research on Similar Robotic Dog Designs

بعد الانتهاء من رسم وتصميم الشكل الأولي لكلبي الروبوتي، قمت بالبحث عن نماذج مختلفة لكلاب روبوتية موجودة مسبقًا؛ وذلك للتأكد من أن التصميم لا ينسخ فكرة أو تصميمًا موجودًا مسبقًا، وللتعرف على الطرق المختلفة المستخدمة في تصميم الروبوتات المشابهة.

وخلال البحث وجدت نموذجًا يحمل بعض التشابه مع تصميمي، خاصة من ناحية الشكل العام وهيكل الجسم. ومع ذلك، توجد اختلافات واضحة في تصميمي، حيث ركزت على تطوير بنية مستوحاة من الغريهاوند، مع تعديلات خاصة في شكل الأقدام، وتصميم المقدمة، وإضافة حساسات في الجزء الأمامي من الجسم، بالإضافة إلى اختلافات في توزيع وشكل المكونات لتحقيق تصميم أكثر ملاءمة لفكرة المشروع.

سيتم إضافة رابط النموذج المشابه للمقارنة وإظهار أوجه التشابه والاختلاف بين التصميمين.

## Similar Existing Project

Petoi OpenCat Quadruped Robot:

https://github.com/PetoiCamp/OpenCat-Quadruped-Robot

----------------------------------------------

# Design Inspiration from the Greyhound

When I read that the project was about designing a robotic dog, the first sentence that came to my mind was—excuse the joke—  
**"All the sighthounds in the valley, get out!"**

For those who are not familiar with the breed, the **Greyhound** belongs to the **Sighthound** group, the same group as the Saluki, although it is a different breed. It has a unique body structure; it is one of the fastest and most efficient dog breeds for running, reaching speeds of around **72 km/h**. It has excellent acceleration, an athletic build, and a streamlined body that resembles a rocket. It also has a flexible skeletal structure and thick paw pads that provide a balance between protection and agility while helping absorb shocks.

It is also characterized by:
- A slim and streamlined body that reduces air resistance (better aerodynamic performance).
- A very tucked-up abdomen that improves agility.
- A balanced body structure designed for speed and efficiency.

For this reason, I based the main structure of my robotic dog on the **Greyhound**, while preserving its most important physical characteristics through:

- A tucked-up abdomen.
- A chest wider than the abdomen with a slight curve.
- An outward-curved back with an arch-like shape.
- Thighs that are wider at both ends and narrower in the middle.
- Legs that are wider at the top and gradually become narrower toward the feet.
- Rounded feet inspired by the shape of Greyhound paws.
- Using **TPU material** to cover the feet due to its flexibility and shock-absorbing properties.
- Adding four pads on the bottom surface of each foot, also made of **TPU**, inspired by Greyhound paw pads to improve stability and reduce impact forces during movement.

## Initial Concept Sketch

<img width="966" height="821" alt="Initial Concept Sketch" src="https://github.com/user-attachments/assets/2e6a0e6a-600c-45bd-87b7-c6391cde498e" />

## Leg and Foot Design

- Adding a **flexible protective TPU layer** on the back and abdomen areas to reduce damage caused by falling, flipping, or sitting, while providing additional protection for the robot’s external structure.

<img width="720" height="610" alt="Leg and Foot Design" src="https://github.com/user-attachments/assets/d53f7f3c-65c6-41d0-99e3-894fa3b4efa9" />

- Designing the front body so that its width gradually decreases toward the head, as well as tapering the rear body, to imitate the Greyhound’s streamlined, rocket-like body shape.
- Adding an **ultrasonic sensor** at the front of the robot to detect nearby obstacles and avoid collisions during movement.

## TPU Protective Layer and Sensor Design

<img width="817" height="658" alt="TPU Protective Layer and Sensor Design" src="https://github.com/user-attachments/assets/ac70e2c6-5317-4525-8e7a-93f91d6198bf" />

The Greyhound’s body structure provides high efficiency by utilizing its mechanical characteristics while maintaining a practical and feasible design. This structure helps **reduce cost, simplify the manufacturing process, and achieve higher reliability and efficiency of the structure** through simpler components and reduced design complexity.

---

# Research on Similar Robotic Dog Designs

After completing the initial sketch and design of my robotic dog, I searched for various existing robotic dog models to ensure that my design did not copy any existing idea or design, and to understand the different approaches used in similar robotic systems.

During my research, I found a model that has some similarities with my design, especially in terms of the overall shape and body structure. However, there are clear differences in my design, as I focused on developing a structure inspired by the Greyhound, with specific modifications in the foot design, front body design, and the addition of sensors at the front of the robot. There are also differences in the arrangement and structure of components to create a design that better fits the project requirements.

The link to the similar model will be added for comparison and to highlight the similarities and differences between both designs.

## Similar Existing Project

Petoi OpenCat Quadruped Robot:

https://github.com/PetoiCamp/OpenCat-Quadruped-Robot
