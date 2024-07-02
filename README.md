# MySQL101-with-compose

## Database Configuration

* สร้างไฟล์ `.env`
```bash
cp .env.example .env
```

* แก้ไขไฟล์ `.env` กำหนดค่าต่าง ๆ ตามต้องการ

```
DB_DATABASE=database_name
DB_USERNAME=db_username
DB_PASSWORD=db_password
```

## Docker Container

```bash
docker-compose up -d
```

## Attach to db container

```bash
docker-compose exec -it db sh
```

* ใช้งาน mysql (ใน sh)
```sh
mysql -u db_username -p
```

## Close Docker Container and down

```bash
docker compose down
```