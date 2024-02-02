## Our Team
# Khusan Khukumov 48598
# Alikhon Hasankhonov 48594
# Erali Choriev 48592

PDF file of the steps
[final_KhusanKhukumov.pdf](https://github.com/IamKhuk/virtual-laravel/files/14138133/final_KhusanKhukumov.pdf)

# Steps

Fist we need to download docker desktop version .
Here is link https://www.docker.com/products/docker-desktop/ 
![1](https://github.com/IamKhuk/virtual-laravel/assets/78492625/0bd954c4-de48-4c74-a7a5-a5c3cbf65e81)

Since I have already install my docker desktop app it is no need to dowload again.

Next step is installing  it on window  and reset your laptop or PS.
![2](https://github.com/IamKhuk/virtual-laravel/assets/78492625/479b7290-1aeb-49e0-a57c-d3799046d7fa)

Here is some image from docker it shows you like defaul window when you come in .

It contains three main tags , containers  images and valuems.

Intall ubuntu 
https://ubuntu.com/tutorials/install-ubuntu-desktop#7-ready-to-install 
![3](https://github.com/IamKhuk/virtual-laravel/assets/78492625/744a0bb7-7d99-404c-8714-0450d5a18b76)

Next Step is installing Laravel 10  PHP framwork with version 8.2 ,

Here is link :

https://laravel.com/docs/10.x 
![4](https://github.com/IamKhuk/virtual-laravel/assets/78492625/a1a3526e-386a-41dc-9bb6-57e304a0d417)

Install with sail with deafult configuration :
![5](https://github.com/IamKhuk/virtual-laravel/assets/78492625/09df6909-0b8d-4806-80c7-1c2f5ac85c8e)

curl -s https://laravel.build/example-app | bash  

Example-app project name let’s rename it to virtual-laravel 

curl -s https://laravel.build/virtual-laravel | bash

Run the code on ubuntu and it require you passwork which is mentioned at the installing process .
After your password request it shows on docker desktop like this 

After  installing 
![6](https://github.com/IamKhuk/virtual-laravel/assets/78492625/637e77df-96df-49ae-aad2-012b5ed154e3)

If you notice we have docker-compose.yml file 
![7](https://github.com/IamKhuk/virtual-laravel/assets/78492625/d4672c9f-b458-4ee5-9a43-0667fbc993e3)

Containers
![8](https://github.com/IamKhuk/virtual-laravel/assets/78492625/978e0ce5-20c7-4c38-98a8-a196520962bb)

Images 
![9](https://github.com/IamKhuk/virtual-laravel/assets/78492625/2b04d7bd-e7d8-46f3-8f4d-8589e520ec9f)

All of them is project requirement packages to run the project on docker virtual box.
![10](https://github.com/IamKhuk/virtual-laravel/assets/78492625/f93601ef-fadc-4d5e-b9ed-3acc34550044)

It shows time how many hours ago it was created . since I have already intalled it gives me this result.

On the container section our Container virtual-laravel project is ready to run  we have two option here to run the application , first one is here second one is on the terminal
![11](https://github.com/IamKhuk/virtual-laravel/assets/78492625/1e8db716-3a11-4432-95ec-1a7312f33907)

Fist Step :
![12](https://github.com/IamKhuk/virtual-laravel/assets/78492625/596f0fb9-8923-484f-b7ec-b884f1b09436)

![13](https://github.com/IamKhuk/virtual-laravel/assets/78492625/2c335edb-3be9-4164-8fc3-98940563d4ae)

Second one is
![14](https://github.com/IamKhuk/virtual-laravel/assets/78492625/cb13c4cc-abd9-40b5-9e29-21eb509d8c39)

Or docker compose up 
![15](https://github.com/IamKhuk/virtual-laravel/assets/78492625/41eb956a-380d-4350-90e4-6cc280b1d9c2)

 phpmyadmin:
        depends_on:
            - mysql
        image: phpmyadmin/phpmyadmin
        environment:
            - PMA_HOST=mysql
            - PMA_PORT=3306
        networks:
            - sail
        ports:
            - 8001:80

Let’s open bws window to see our PHP my andim and our project :
![16](https://github.com/IamKhuk/virtual-laravel/assets/78492625/081564de-5080-49bc-968c-d1c8e9951577)

It is already running 

Login :  sail 
Password : password 

mysql:
        image: 'mysql/mysql-server:8.0'
        ports:
            - '${FORWARD_DB_PORT:-3306}:3306'
        environment:
            MYSQL_ROOT_PASSWORD: '${DB_PASSWORD}'
            MYSQL_ROOT_HOST: '%'
            MYSQL_DATABASE: '${DB_DATABASE}'
            MYSQL_USER: '${DB_USERNAME}'
            MYSQL_PASSWORD: '${DB_PASSWORD}'
            MYSQL_ALLOW_EMPTY_PASSWORD: 1
        volumes:

![17](https://github.com/IamKhuk/virtual-laravel/assets/78492625/2167ab8e-fe98-4a58-990c-ca056b0e9c6e)

Let’s see our project on localhost :
![19](https://github.com/IamKhuk/virtual-laravel/assets/78492625/b82d4c55-71cf-463a-a258-ce3ced954918)

We can also change something .
![20](https://github.com/IamKhuk/virtual-laravel/assets/78492625/3d34f213-bdda-47da-8aef-e1bb061893d4)

![21](https://github.com/IamKhuk/virtual-laravel/assets/78492625/54e6ec3f-4527-4fb7-91e7-b57387ba13a8)

If we want to working with terminal later on , open it 
![22](https://github.com/IamKhuk/virtual-laravel/assets/78492625/ce974db1-525d-46d5-a2c8-f91ba8b3b821)

On container section :
![23](https://github.com/IamKhuk/virtual-laravel/assets/78492625/568ffa4d-9525-4e7c-8611-f82a7422e9cf)

Let’s add extra functionalities for this project to make a usefull app .
![24](https://github.com/IamKhuk/virtual-laravel/assets/78492625/ffe854a8-acb2-43aa-9063-8b6015246206)

This user registration tables in database :
![25](https://github.com/IamKhuk/virtual-laravel/assets/78492625/f88b4134-44eb-4c91-9ae4-cfd0cc0a945e)

Extra tables is here :
![26](https://github.com/IamKhuk/virtual-laravel/assets/78492625/dc435b59-a952-41f8-b317-08d1c792631d)

Let’s fill the database with fake data by writing  php artisan db:seed 
![27](https://github.com/IamKhuk/virtual-laravel/assets/78492625/7d75a9cf-a16e-4793-95d2-961b018e6e7c)

Just one user exists here who is owner of the web app :
![28](https://github.com/IamKhuk/virtual-laravel/assets/78492625/9415413a-f50e-428d-b117-bc8163567413)

Login : admin@domain.com
Password: password ;

Admin can see this only  and add books to web app to show public .
![29](https://github.com/IamKhuk/virtual-laravel/assets/78492625/3264fe67-9e0c-4f75-a1b3-c62d3d681156)

![30](https://github.com/IamKhuk/virtual-laravel/assets/78492625/04d1c8f8-0412-4e38-ab87-28acb7e56492)
![32](https://github.com/IamKhuk/virtual-laravel/assets/78492625/e86bb01e-5719-40a3-9398-726208ae5cd3)
![31](https://github.com/IamKhuk/virtual-laravel/assets/78492625/e4c140ff-9634-4011-b986-d352c7643f15)

Index :
![33](https://github.com/IamKhuk/virtual-laravel/assets/78492625/128b0433-acb8-4a6b-9f57-78369c0c1354)

Create :
![34](https://github.com/IamKhuk/virtual-laravel/assets/78492625/c605257c-b6e4-49ca-a1f3-851205fa9fd6)

View 
![35](https://github.com/IamKhuk/virtual-laravel/assets/78492625/1060caf8-07d9-40a6-a8f4-a0702e6db3ea)

Edit :
![36](https://github.com/IamKhuk/virtual-laravel/assets/78492625/0e6f82d1-5e30-43c8-bf9a-9c08f10cad78)

Delete :
![37](https://github.com/IamKhuk/virtual-laravel/assets/78492625/021850d9-8650-40a9-966f-07af9a6c34e1)

Here is our books in database :
![38](https://github.com/IamKhuk/virtual-laravel/assets/78492625/1b25cded-89c9-409f-9afb-4e3dc366f1c9)

Everything is working correctly :) 

# Thank you , I have learned so many thing on Cloud-oriented web application during the session . 

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
# cloud-laravel
# cloud-laravel
# cloud-laravel
