# テクノロジー（藤原） 11/1授業

```
(ここに実行ログをコピペする)
[1] pry(main)> num = 2 
=> 2
[2] pry(main)> if num % 2 == 0
[2] pry(main)*   puts "偶数です"
[2] pry(main)* end  
偶数です
=> nil
[3] pry(main)> arr = []
=> []
[4] pry(main)> (1..20).each do |num|
[4] pry(main)*   if num % 2 == 0
[4] pry(main)*     puts "偶数です"
[4] pry(main)*     arr << num 
[4] pry(main)*   end  
[4] pry(main)* end    
偶数です
偶数です
偶数です
偶数です
偶数です
偶数です
偶数です
偶数です
偶数です
偶数です
=> 1..20
[5] pry(main)> arr = []
=> []
[6] pry(main)> (1..20).each do |num|
[6] pry(main)*   if num % 2 == 0  
[6] pry(main)*     puts "偶数です:#{num}"    
[6] pry(main)*     arr << num 
[6] pry(main)*   end  
[6] pry(main)* end  
偶数です:2
偶数です:4
偶数です:6
偶数です:8
偶数です:10
偶数です:12
偶数です:14
偶数です:16
偶数です:18
偶数です:20
=> 1..20
[7] pry(main)> arr
=> [2, 4, 6, 8, 10, 12, 14, 16, 18, 20]
[8] pry(main)> num = 1000
=> 1000
[9] pry(main)> if num >= 1500 
[9] pry(main)*   puts "送料無料です"
[9] pry(main)* elsif 0 < num && num < 1500   
[9] pry(main)*   puts "送料300円です"
[9] pry(main)* else   
[9] pry(main)*   puts "入力が間違ってます"
[9] pry(main)* end  
送料300円です
=> nil
[10] pry(main)> (1..20).map do |num|
[10] pry(main)*   puts num
[10] pry(main)* end  
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
=> [nil,
 nil,
 nil,
 nil,
 nil,
 nil,
 nil,
 nil,
 nil,
 nil,
 nil,
 nil,
 nil,
 nil,
 nil,
 nil,
 nil,
 nil,
 nil,
 nil]
[11] pry(main)> map
NameError: undefined local variable or method `map' for main:Object
Did you mean?  tap
from (pry):31:in `__pry__'
[12] pry(main)> num = rand 3 
=> 0
[13] pry(main)> case num 
[13] pry(main)* when 0  
[13] pry(main)*   puts "吉です"
[13] pry(main)* when 1  
[13] pry(main)*   puts "凶です"
[13] pry(main)* else  
[13] pry(main)*   puts "大凶です"
[13] pry(main)* end  
吉です
=> nil
[14] pry(main)> def trisngle(b, h)
[14] pry(main)*   result = b * h / 2.0
[14] pry(main)*   return result
[14] pry(main)* end  
=> :trisngle
[15] pry(main)> trisngle(11, 9)
=> 49.5
[16] pry(main)> trisngle 11, 9                                                  
=> 49.5
[17] pry(main)> [1, 2, 3].empty?
=> false
[18] pry(main)> arr = 
[18] pry(main)* []
=> []
[19] pry(main)> arr = []
=> []
[20] pry(main)> arr.empty?
=> true
[21] pry(main)> name = gets 
My name is Jack Haboc        
=> "My name is Jack Haboc\n"
[22] pry(main)> name.chomp!
=> "My name is Jack Haboc"
[23] pry(main)> name
=> "My name is Jack Haboc"
[24] pry(main)> 10.times do |i|
[24] pry(main)*   print i, ","
[24] pry(main)* end  
0,1,2,3,4,5,6,7,8,9,=> 10
[25] pry(main)> a = ["リンゴ", "ミカン", "ブドウ"]
=> ["リンゴ", "ミカン", "ブドウ"]
[26] pry(main)> a.each do |item|
[26] pry(main)*   puts "美味しい" + item + "だよ"
[26] pry(main)* end  
美味しいリンゴだよ
美味しいミカンだよ
美味しいブドウだよ
=> ["リンゴ", "ミカン", "ブドウ"]
```