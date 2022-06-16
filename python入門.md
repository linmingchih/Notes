#### 變數
變數一般由英文字母，數字及底線組成，用來儲存資料
        
        position = (1.3, 2.6, 5.4)
        substrate_height = '3.3 mil'
        layer1_material = ('copper', '4 mil',)

以上的position, substrate_height, layer1_material皆為變數。

#### 基本資料型態
1. 整數

        vias_count = 104
        i = 4
    
2. 浮點數

        width = 2.3
        spacing = 1.4
3. 複數

        Etheta = 1+3j
        Ephi = -3-4j
5. 字串

        layer_name = 'GND'
        width = "10mil"
        
注意雙引號""跟''單引號都可以用來定義字串

4. 布林

        is_metal = True
        enabled = False

#### 基本資料結構
變數不只可以指向基本資料，也可以指向資料結構，常用的基本資料結構有以下幾種：
1. list，由中括號組成：

        layers = ['top', 'pwr', 'gnd', 'bottom']
        nets = ['dq0', 'dq1', 'dq3']
        
2. tuple，由小括號組成：

        location = (1 ,2, 1)
        layer_property = ('top', 1.1, 'copper', True)

3. dictionary，由大括號組成：

        layer_thickness = {'top':1.3, 'bottom':1.4}
        dielectric_info = {'fr4_A':(4.3, 0.02), 'fr4_B':(3.9, 0.015), 'fr4_C':(2.8, 0.021)}
        
#### 類別與物件
類別是進階的資料型態，一般由開發者自訂，以下是一個簡單的class定義：

        class fuel_tank:
            def __init__(self):
                self.fuel = 0
                
            def get_fuel_amount(self):
                return self.fuel
                
            def fill_fuel_amount(self, liter=0)
                self.fuel += liter

        class car:
            def __init__(self, name, color):
                self.name = name
                self.color = color
                self.fuel_tank = fuel_tank()
                self.speed = 0
            
            def set_speed(self, price):
                self.speed = speed
            
            def get_speed(self):
                return self.speed
                
編寫PyAEDT腳本很少需要自行開發類別及物件，但是一定要會使用他們，因為pyAEDT當中所有可以操控的動作都必須透過物件來完成。
因為整個AEDT就是一個由很多子物件構成的複雜物件，開發者必須清楚知道每個子物件的位置及對應的屬性及函數。

開發過程便是要設定

                
               
