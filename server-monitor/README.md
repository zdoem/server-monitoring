# server-monitoring | การติดตั้งระบบ Monitor Server อย่างง่ายด้วย Docker (grafana + prometheus + node exportor )

### ความต้องการเบื้องต้นของระบบ
    docker
    docker-compose
    git

### คู่มือแบบที่ 1

    git https://github.com/zdoem/server-monitoring/tree/master
    cd server-monitor
    chmod -R 777 grafana
    
#### จากนั้นทดสอบ ว่ามันทำงานได้ไหม

    docker-compose up

จะเจอหน้าจอดำ ๆ กะข้อความอิหยังบุ๊ แหล่นล้าย ๆ ประมาณนี้


จากนั้นนั้น เปิด browser ที่เราถนัด ใส่ url = http://ip_server:3000

    ip_server = ip ของ server ที่เราติดตั้งตัว server monitor นี้

จะเจอหน้าจอ login
    
    user = admin
    password = admin
    
จากนั้น เลือกกราฟ ที่จะเราจะ monitor ครับ ผมใส่มาให้แล้ว 2 กราฟคือ
1. Node Exporter Full ไว้สำหรับ monitor ตัวเครื่อง server ของเราครับ

การเลือกแสดงกราฟ ครั้งแรก ไปที่ 
