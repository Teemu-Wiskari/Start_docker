# Задание 2

Запуск контейнера:
- заменить значения переменных в файле reast_api_container/stocks_products/.env
- собрать образ командой
  
      docker image build rest_api_container/ --tag=teemu_wiskari2

- запустить контейнер:

        docker run --name=teemu_wiskari2 -d -p 6060:6060 teemu_wiskari2

