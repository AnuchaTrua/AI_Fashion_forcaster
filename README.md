# AI_Fashion_forcaster
AI that predict your fashion stock in future

วิธีการใช้งาน (การเปิด project)
1.โหลดไฟล์ zip ทั้งสองไฟล์ใน repo (AI_fashion_forcaster_model-main.zip และ fashion-frontend-main.zip)ทำการแตกไฟล์ทั้งสองและเปิดทั้ง 2 folder ใน vscode
2.ใน folder frontend (fashion-frontend-main.zip) เมื่อเปิดใน vscode แล้วจากนั้นเปิด terminal ของ vscode แล้วพิมพ์ npm install รอโหลดเสร็จ
3.จากข้อ 2 หากโหลดเสร็จแล้วให้พิมพ์ใน terminal ต่อว่า npm run dev เพื่อรันจากนั้นจะได้ link เว็ปใน terminal ให้ทำการก็อปไปใส่ browser
4.ฝั่ง backend (AI_fashion_forcaster_model-main.zip) เมื่อเปิดเสร็จเข้า terminal ของ vscode จากนั้นพิมพ์ uvicorn fastapi_app:app --reload เพื่อรันโมเดลและ backend
5.เมื่อข้อ 4 รันสำเร็จให้กลับไปที่หน้าเว็ปที่เปิดไว้ก็สามารถใช้งานได้ทันทีเลย

วิธีการใช้งาน (การใช้เว็ป)
1.ในหน้าเว็ปก่อนทำนายคุณต้องเลือกสินค้าก่อน
2.เมื่อลเลือกสินค้าเสร็จสามารถระบุ ราคา , จำนวนที่เหลืออยู่ , ส่วนลด , ระยะเวลา (7,30วัน) ทั้งหมดนี้หากไม่ได้ระบุจะดึงข้อมูลเดิมจาก database(csv) มาใช้ ยกเว้นวันที่ base จะเป็น 7 วัน

โดยโครงสร้างไฟล์ใน backend ไฟล์ train หลักคือ 02_train_lstm.ipynb
