Les bases du PHP

```php
<?php
    /**
     * Ma première classe PHP
     */
    class MonMessage{
        public function SayHello() : void{
            echo $this->GetMessage();
        }
        
        private function GetMessage() : string{
            return 'Hello';
        }
    }
    
    MonMessage->SayHello();
```