# docker_laravel_env_hyahha
�ȒP�Ɍ����ƁA���U��Laravel�̊�����ɓ���܂��B</br>

</br>


## ����
Windows10�ō\�����܂����ALaravel�h�b�J�[���ł��B</br>
���e��
nginx</br>
php </br>
mysql</br>
</br>
�|�[�g�@NGINX -> 80</br>
	MYSQL -> 3306</br>
�������|�[�g�����Ƌ������Ă���G���[�ɂȂ�܂��B</br>
</br>
���g���u���V���[�e�B���O</br>
Laravel 5.4: Fatal error: Uncaught Error: Class 'Illuminate\Foundation\Application' �̃G���[</br>
$ composer install</br>
$ composer dump-autoload</br>
�ŉ���
</br>
</br>
500�G���[���o��</br>
env���Ȃ������B�B�B</br>
�Ȃ����.env.example���R�s�[���ē����ʒu��.env�Ƀ��l�[�����ē\��t��</br>
</br>
RuntimeException ���ł�</br>
key �𐶐�����</br>
php artisan key:generate</br>

</br>


## �g����


</br>
�t�@�C���ʒu�́ALaravel�t�@�C����iot�Ƃ��Ă����Ă�������</br>
</br>
laravel_project</br>
������ iot (Laravel�t�@�C��)</br>
������ docker-compose.yml</br>
������ docker-nginx</br>
��   ������ Dockerfile</br>
��   ������ default.conf</br>
������ docker-php</br>
    ������ Dockerfile</br>
</br>


### Install
```sh
git clone https://github.com/umaxiaotian/docker_laravel_env_hyahha.git
cd docker_laravel_env_hyahha
docker-compose build
docker-compose up -d

����Ŏg����͂��ł��B