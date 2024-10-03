# Задание 1

Создание образа:

    docker image build . --tag=teemu_wiskari

Запуск контейнера:

    docker run --name=teemu_wiskari -d -p 7771:80 teemu_wiskari
