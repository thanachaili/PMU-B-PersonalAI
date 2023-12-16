# PMU-B-PersonalAI
> :star2: thanachai Liewkhonkaen

---

## 1. xPore: An AI-Powered App for Bioinformaticians :point_right: [Click here](https://github.com/thanachaili/PMU-B-PersonalAI/blob/1fcf42e765ac7965ce70262e511f909e29881f21/GMM_thanachai.ipynb) 
---
    สิ่งที่ทำ
---
  - 1.สกัดพารามิเตอร์ (Q1, Q2, Q3) จาก GMM:
    *weights = gmm.weights_: สกัดค่าน้ำหนักของส่วนประกอบจาก GMM ที่ฝึกสอนไว้
    *means = gmm.means_: สกัดค่าค่าเฉลี่ยของส่วนประกอบจาก GMM ที่ฝึกสอนไว้
    *covariances = gmm.covariances_: สกัดเมทริกซ์ความแปรปรวนของส่วนประกอบจาก GMM ที่ฝึกสอนไว้
    จากนั้นโดยสำหรับGMMที่มีส่วนประกอบสองอัน (ที่ระบุโดย n_components=2) โค้ดจะแยกและกำหนดค่าน้ำหนัก (weights), ค่าเฉลี่ย (means), และค่าส่วนประกอบของความแปรปรวน (covariances) ไปยังตัวแปร w1,w2,mu1,mu2,sd1,และsd2
  - 2.พิมพ์สมการของ Gaussian Mixture Model:
    *print('p(x) = %.2f*Normal(%.2f,%.2f) + %.2f*Normal(%.2f,%.2f)' % (w1, mu1, sd1, w2, mu2, sd2)): พิมพ์สมการของ Gaussian Mixture Model ที่ได้สกัดมาโดยใช้พารามิเตอร์ที่ได้จาก GMM ออกมาแสดงผล
  - 3.แสดงผลข้อมูลและการกระจายที่ได้จากการสกัด (Q4):
    *viz([list(data1)] + [list(data2)], [mu1, mu2], [sd1, sd2]): เรียกใช้ฟังก์ชันการแสดงผล viz() โดยส่งข้อมูล (data1 และ data2) และค่าเฉลี่ยและค่าส่วนประกอบของความแปรปรวนที่ได้สกัดมา (mu1, mu2, sd1, sd2) เพื่อแสดงผล       ข้อมูลและการกระจายของการแจกแจงปกติที่ได้สกัดมา
---
