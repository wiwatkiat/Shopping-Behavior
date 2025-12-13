# Shopping-Behavior
"The store has declining sales and lacks exponential growth. The current marketing strategy focuses on offering discounts and a subscription system to attract customers."
1. Problem Statement / Background (ที่มาและความสำคัญ)
ในปัจจุบัน ธุรกิจค้าปลีกเผชิญกับการแข่งขันสูง การเข้าใจพฤติกรรมผู้บริโภคจึงเป็นหัวใจสำคัญ จากการสังเกตเบื้องต้นพบว่าการทำการตลาดแบบหว่านแห (Mass Marketing) เช่น การแจกส่วนลด (Discount) หรือระบบสมาชิก (Subscription) อาจไม่ได้สร้างผลตอบแทนที่คุ้มค่าสูงสุด และยังขาดความชัดเจนว่าปัจจัยใดกันแน่ที่ขับเคลื่อนยอดขาย (Purchase Amount) และความภักดีของลูกค้า (Loyalty) อย่างแท้จริง

2. Objectives / SMART Objectives (วัตถุประสงค์)
S (Specific): เพื่อวิเคราะห์ความสัมพันธ์ระหว่างข้อมูลประชากร (Demographics) และพฤติกรรมการซื้อ กับยอดการใช้จ่ายและสถานะสมาชิก

M (Measurable): วัดผลโดยใช้ค่าสัมประสิทธิ์สหสัมพันธ์ (Correlation Coefficient) และค่า P-value เพื่อดูระดับนัยสำคัญทางสถิติ

A (Achievable): สามารถทำได้จริงโดยใช้ข้อมูล Transaction History จำนวน 3,900 แถวที่มีอยู่

R (Relevant): ผลลัพธ์ที่ได้จะนำไปสู่การปรับปรุงกลยุทธ์ "Tiered Discount" และ "Lead Scoring"

T (Time-bound): สรุปผลการวิเคราะห์และนำเสนอโมเดลภายในระยะเวลาที่กำหนด

3. Analytical Questions (คำถามเชิงวิเคราะห์)
อายุ (Age) และยอดซื้อสะสม (Previous Purchases) มีความสัมพันธ์กับยอดใช้จ่ายต่อบิล (Purchase Amount) หรือไม่?

คะแนนรีวิว (Review Rating) มีความสัมพันธ์กับจำนวนครั้งที่ซื้อซ้ำหรือไม่?

การมีส่วนลด (Discount) มีความสัมพันธ์กับยอดการซื้อที่สูงขึ้นจริงหรือไม่?

4. Data Sources (แหล่งข้อมูล)
Dataset: Shopping_behavior_updated (1).csv

จำนวนข้อมูล: 3,900 Records

ลักษณะข้อมูล: ข้อมูลการทำธุรกรรมรายบุคคล (Transaction Data) ประกอบด้วยข้อมูลเชิงปริมาณ (เช่น ยอดซื้อ, อายุ) และข้อมูลเชิงคุณภาพ (เช่น เพศ, หมวดสินค้า)

5. Data Cleansing (การทำความสะอาดข้อมูล)
Missing Values: ตรวจสอบค่าสูญหาย และจัดการ (Drop/Impute) หากพบ

Duplicates: ตรวจสอบและลบข้อมูลซ้ำซ้อนเพื่อป้องกันความคลาดเคลื่อน

Data Type Conversion: แปลงข้อมูล Categorical เป็น Numerical สำหรับการวิเคราะห์ทางสถิติ (เช่น Subscription: Yes=1, No=0 / Gender: Male=0, Female=1)

6. Exploratory Data Analysis (EDA)
