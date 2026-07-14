# Mechanical Design of a Simple Greyhound-Inspired Robot Dog

# 1. Body and Chassis Design | تصميم الجسم والهيكل

The robot body was designed to resemble the overall shape of a Greyhound while maintaining a simple, lightweight structure suitable for 3D printing.

تم تصميم جسم الروبوت ليحاكي الشكل العام لكلب الغريهاوند مع المحافظة على بساطة التصميم وخفة الوزن وسهولة تصنيعه باستخدام الطباعة ثلاثية الأبعاد.

## Body Dimensions | أبعاد الجسم

- **Body Length | 22 cm
- **Body Width | 8.5 cm
- **Body Height | 6.5 cm

---

## Body Material | مادة الهيكل

The body and legs are manufactured using **ABS plastic**.

تم اختيار **ABS** كمادة أساسية لتصنيع الجسم والأرجل.

### Why ABS? | سبب اختيار ABS

- Lightweight to reduce the load on the motors.
- Better impact resistance than PLA.
- High structural rigidity.
- Suitable for 3D printing.
- Lower cost than aluminum.

- خفيف الوزن مما يقلل الحمل على المحركات.
- يتحمل الصدمات بشكل أفضل من PLA.
- صلب بما يكفي للحفاظ على ثبات الهيكل.
- مناسب للطباعة ثلاثية الأبعاد.
- أقل تكلفة من الألمنيوم.

---

## Protective TPU Layers | طبقات الحماية

### Upper Protective Layer (Back) | طبقة الظهر

A TPU layer was added to the robot's back to absorb impacts in case the robot flips over.

تمت إضافة طبقة TPU على الظهر من أجل:

- امتصاص الصدمات.
- حماية هيكل ABS.
- تقليل احتمالية تشقق الجسم.

### Bottom Protective Layer (Belly) | طبقة البطن

A TPU layer was added underneath the body to protect the robot during ground contact.

تمت إضافة طبقة TPU في البطن من أجل:

- امتصاص الصدمات.
- حماية الجزء السفلي.
- تقليل انتقال الاهتزازات.
- السماح بمرونة بسيطة أثناء الحركة.

---

# 2. Leg Design | تصميم الأرجل

The legs were designed to imitate the proportions of a Greyhound while maintaining low weight and high strength.

تم تصميم الأرجل بحيث تحاكي أرجل كلب الغريهاوند مع المحافظة على خفة الوزن والمتانة.

## Leg Dimensions | أبعاد الأرجل

- **Upper Leg (Thigh) |6 cm
- **Lower Leg | 6 cm
- **Foot | 3 × 2.5 cm

### Thigh Design | تصميم الفخذ

The thigh is:

- Thick near the hip joint.
- Narrow in the middle.
- Thick again near the knee joint.

تم تصميم الفخذ ليكون:

- سميكًا عند مفصل الورك.
- نحيفًا في المنتصف.
- سميكًا مرة أخرى عند مفصل الركبة.

### Reason | السبب

- Higher strength around the joints.
- Lower overall weight.
- Better load distribution.
- Reduced rotational inertia.

- زيادة القوة عند المفاصل.
- تقليل الوزن.
- تحسين توزيع الأحمال.
- تقليل عزم القصور الذاتي.

### Foot Design | تصميم القدم

The foot consists of two parts.

تتكون القدم من جزأين.

**Core**

Material: **ABS**

Function:

- Supports the robot weight.
- Connects the foot to the leg.
- Provides structural rigidity.

- تحمل وزن الروبوت.
- تثبيت القدم مع الساق.
- المحافظة على صلابة القدم.

**Outer Layer**

Material: **TPU**

Function:

- Increases friction.
- Prevents slipping.
- Absorbs impacts.

- زيادة الاحتكاك.
- تقليل الانزلاق.
- امتصاص الصدمات.

---

# 3. Degrees of Freedom (DOF) | درجات الحرية

Each leg has two joints.

كل رجل تحتوي على مفصلين.

- **Hip:** Forward and backward movement.
- **Knee:** Flexion and extension.

- Hip: حركة أمامية وخلفية.
- Knee: ثني وفرد.

- Degrees of Freedom per leg: **2**
- Number of legs: **4**
- Total Degrees of Freedom: **8 DOF**

تم اختيار درجتي حرية فقط لكل رجل لتبسيط التصميم وتقليل عدد المحركات والتكلفة.

---

# 4. Motor Selection | اختيار المحركات

Selected Motor:

**MG996R Servo Motor**

Specifications:

- Type: Servo
- Voltage: 4.8–6 V
- Torque: 11 kg·cm
- Weight: 55 g

### Why MG996R?

- Provides torque higher than the required value.
- Suitable for the robot size.
- Easy PWM control.
- Low cost.
- Widely available.
- Reliable for repeated walking.

- يوفر عزمًا أعلى من المطلوب.
- مناسب لحجم الروبوت.
- سهل التحكم.
- منخفض التكلفة.
- متوفر.
- يتحمل الحركة المتكررة.

---

# 5. Preliminary Torque Calculation | حساب العزم المبدئي

Torque Equation:

```
T = F × L
```

Force Equation:

```
F = m × g
```

Assuming:

```
m = 0.09 kg
g = 9.81 m/s²
```

```
F = 0.09 × 9.81 = 0.883 N
```

```
L = 6 cm = 0.06 m
```

```
T = 0.883 × 0.06 = 0.053 N·m
```

Safety Factor = 2

```
T = 0.106 N·m
```

Converted:

```
1.08 kg·cm
```

The MG996R provides **11 kg·cm**, which is much higher than the required torque.

---

# 6. Stability and Center of Gravity | الثبات ومركز الجاذبية

The battery and electronics are placed near the center of the body to keep the center of gravity inside the support polygon.

تم وضع البطارية والإلكترونيات بالقرب من منتصف الجسم للحفاظ على مركز الجاذبية داخل منطقة الارتكاز.

Advantages:

- Better stability.
- Reduced tipping.
- Improved balance.

- زيادة الثبات.
- تقليل الانقلاب.
- تحسين الاتزان.

---

# 7. Proposed Walking Gait | طريقة المشي

Selected Gait:

**Crawl Gait**

Walking Sequence:

1. Front Right Leg.
2. Rear Left Leg.
3. Front Left Leg.
4. Rear Right Leg.

Reasons:

- High stability.
- Easy implementation.
- Suitable for small quadruped robots.

- أكثر ثباتًا.
- سهلة البرمجة.
- مناسبة للروبوتات الصغيرة.

---

# 8. Expected Mechanical Challenges | المشاكل الميكانيكية المتوقعة

- High motor loads.
- Foot slipping.
- Body vibration.
- Battery consumption.
- Joint wear.
- Screw loosening.
- Loss of balance.
- Impact during robot flipping.

- زيادة الحمل على المحركات.
- انزلاق القدم.
- اهتزاز الهيكل.
- استهلاك البطارية.
- احتكاك المفاصل.
- ارتخاء البراغي.
- فقدان التوازن.
- تعرض الجسم للصدمات عند الانقلاب.

---

# Materials | المواد

- Body: ABS
- Legs: ABS
- Foot Core: ABS
- Foot Outer Layer: TPU
- Back Protective Layer: TPU
- Belly Protective Layer: TPU
- Shafts: Steel
- Joints: Ball Bearings

- الجسم: ABS
- الأرجل: ABS
- قلب القدم: ABS
- غلاف القدم: TPU
- طبقة الظهر: TPU
- طبقة البطن: TPU
