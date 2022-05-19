![](https://github.com/mr687/mr687/blob/main/header.png)

```php
// ~/.tmp/Profile/Intro.php

<?php

namespace Mr687\Daphinokio;

use Facades\Mr687\Daphinokio\Media;
use Facades\Mr687\Daphinokio\Profile;
use Facades\Mr687\Daphinokio\Development;

class Intro
{

  /**
  * __invoke()
  * 
  * @params array $learning
  * @return error
  */
  public function __invoke(array $learning)
  {
    Profile::name = 'Davi Nomoeh Dani';
    Profile::alias = 'daphinokio'; // 'phi' === 'vi'
    Profile::email = 'davinomoehdanino@gmail.com'; // Email address is already taken
    
    Media::instagram = Media::twitter = '@daphinokio';
    
    Development::langs = [
      'backend' => 'php:laravel|javascript:node-js|python',
      'frontend' => 'php:livewire|javascript:react-js,vue-js',
      'database' => 'postgresql|mysql|mongodb|sqlite'
    ];
    Development::misc = [
      'devops' => 'aws:ec2,rds,lightsail,s3|heroku',
      'tools' => 'git|postman|vscode',
      'os' => 'mac-os'
    ];
    Development::experience = carbon('2018-01-01')->diffInYears();
    
    return $this($learning);
  }
  
}

```

```
- 🥱 I am currently working on javascript.
- 🚀 Available for Freelance projects opportunities.
```

![](https://visitor-badge.laobi.icu/badge?page_id=mr687.mr687)
