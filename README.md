# docker-command

* docker images *คำสั่งดู image*
* docker run image_name *คำสั่งรัน image*
* docker verion *คำสั่งเช็คเวอร์ชั่น สถาะนะ ของ docker*
* docker history image_name *คำสั่งเช็คว่าเคยรัน image นี้ไว้เมื่อไรและมีกี่เลเยอร์*
* docker ps *คำสั่งลิสต์ containers* 
* docker run container container_name *คำสั่งรัน container*
* docker network creat networl_name *คำสั่งสร้าง network*
* docker network ls *คำสั่งลิสต์ network*
* docker rm containner_id *คำสั่งลบ container ใช้เลข 4 หลักแรก*


# docker-compose

* docker-compose up -d *run container จากไฟล์ docker-compose.yaml*
* docker-compose dowm *stop container จากไฟล์ docker-compose.yaml*
- ไฟล์ docker-compose ทำหน้าที่แทนการใช้ CLI เราสามารถเพิ่ม คำสั่งต่างๆ รวมถึงกำหนด port network เข้าไปในไฟล์ได้
    - version : *กำหนดเวอร์ชั่นของ docker compose*
    - service : *ภายใน นี้จะมี image อะไรบ้าง รวมถึงการ setting ต่างๆ*
    - container_name : *ใช้ตั้งชื่อของ containner* 
    - networks : *กำหนด network*
    - ports : *กำหนด port ของแต่ละ image*
    - depends_on : *ให้ image ouh ทำงานบนอะไร*