// para resolver problemas de permissão do configuration.php

    sudo touch configuration.php
    sudo chmod 777 configuration.php

// apos instalação passar para: 

    sudo chmod 755 configuration.php

// para resolver problemas de permissão para upload

    sudo chown -R www-data:www-data .

// Encontrar no texto dos arquivos, por exemplo o texto jquery.min.php:

    grep -r jquery.min.php | awk -F\: '{ print $1 }'
