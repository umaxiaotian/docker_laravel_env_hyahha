# docker_laravel_env_hyahha
�ȒP�Ɍ����ƁA���U��Laravel�̊�����ɓ���܂��B


## Description
Windows10�ō\�����܂����ALaravel�h�b�J�[���ł��B
���e��
nginx
php 
mysql

�|�[�g�@NGINX -> 80
	MYSQL -> 3306
�������|�[�g�����Ƌ������Ă���G���[�ɂȂ�܂��B

���g���u���V���[�e�B���O
Laravel 5.4: Fatal error: Uncaught Error: Class 'Illuminate\Foundation\Application' �̃G���[
$ composer install
$ composer dump-autoload
�ŉ���


500�G���[���o��
env���Ȃ������B�B�B
�Ȃ����.env.example���R�s�[���ē����ʒu��.env�Ƀ��l�[�����ē\��t��

RuntimeException ���ł�
key �𐶐�����
php artisan key:generate


## Usage
### Install
```sh
git clone https://github.com/umaxiaotian/docker_laravel_env_hyahha.git
cd docker_laravel_env_hyahha
docker-compose build
docker-compose up -d

����Ŏg����͂��ł��B