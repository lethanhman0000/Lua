-- ( day la comment )
--[[
co the viet nhieu dong comment o day
]]

--in 1 thu gi do ra man hinh
print ("xin chao the gioi !!!")

--khai bao gia tri cho 1 bien
local name = "johan"
local so = 10 -- day la gan gia tri cho a bang 10
local name1= nil --day la gia tri bang 0, khong co gi 

-- in bien ra man hinh
print (name)

--cong 2 gia tri chuoi string lai voi nhau "string 1" .. "string 2"
-- <..> day la dau cong 2 chuoi lai voi nhau
print ("string1".. " ".."string2")

local a = 10
print (a) -- neu ban in ra no se bang 10, nhung neu ban bo di so 10 thi no se ra nil
-- nghia la bien no khong co gia tri hoac nghia gi ca, no khong duoc gan
local b
print (b)

--neu nhu ban in ra so thi sao ?
print (5)
--khao bao bien
local so1 = 5
print (so1 .. 5)

--[[
cau lenh if else
if < dieu kien > then
elseif < dieu kien > then
 < lenh thuc thi >
 else < dieu kien > then
 < lenh thuc thi >
end
]]
-- chung ta se viet chuuong trinh in ra dong chu
-- ban du tuoi de vao web !!! ( tren 18 tuoi )

tuoi = 0 --cai nay chung ta cho tuoi bang 10
dieukien = 18 -- day la dieu kien de vao web
if tuoi > dieukien then
  print ("Hop le, chuc ban xem phim vui ve")
elseif tuoi < dieukien then
  print ("Ban khong du tuoi, vui long quay lai sau !!!")
  else
    print ("khong xac dinh duoc do tuoi cua ban !!!")
    end

--[[
cau lenh lap while ... do
while < dieu kien > do
< lenh thuc thi > 
end
]]
-- chung ta se viet chuog trinh in ra 10 dong xin chao 
i = 1 
while i <= 10 do
  print ("xin chao")
  i = i + 1
end
-- dau tien i se co gia tri la 1, no xet duyet dieu kien, neu be hon hoac bang 
-- 1 thi in ra chu xin chao, no duyet den khi nao i <=1 thi thoi, con neu i cu bang 1 
-- hoai thi chuong trinh se chay hoai ko dung. 

--[[
cau lenh lap for .. do 
for <gia tri bat dau>, <gia tri ket thuc>, <buoc nhay> do
< lenh thuc thi >
end
]]
-- chuong trinh in ra 10 dong xinchao
for i=1, 10, 1 do
  print ("xinchao")
end

--[[
ham 
function < ten ham > ()
< lenh thuc thi >
end
cach dung :

<ten ham>() co the goi o bat ki noi nao trong chuogn trinh, vi ham
duoc tao ra la de dung lai nhieu lan chuc nang cua 1 doan code, chu khong phai 
code lai nhieu lan
]]
--in ra xinchaovietnam
function inraxinchaovietnam() -- tao ra ham inraxinchaovietnam
  print ("xinchaovietnam")
end
inraxinchaovietnam()

--viet ham a + b , a = 5, b = 10
function tong(a, b) -- ham co the viet them thao so vao, trong day la tham so a va b  
  print (a + b) -- luc nay a va b la 2 bien cuc bo co trong ham nay, khi ra khoi ham
  -- thi 2 bien a va b se bien mat, no chi co tac dung khi o trong ham
end
tong(5, 10) -- chung ta co the chen gia tri cho tham so trong ham, ket qua bang 15

-- bien toan cuc (global) va bien cuc bo(local)
-- 
--bien cuc bo- nghia la no co gia tri rieng cho no trong 1 ham nhat dinh, neu nhu ta 
-- dung local truoc khi dat bien, nghia la trong ham do no mang gia tri cua bien do
--no dang nam trong ham inray()

x = "x"
print(x)
function inray()
  local x = "y"
  print (x)
end
inray()
print(x)

-- vi du ve return trong ham
function ketqua1(a, b)
  return a + b
end
function ketqua2(kq1)
  return kq1 * 2
end
 kq1= ketqua1(5, 5)
 kq2= ketqua2(kq1)
print(kq1) 
print(kq2)
-- tu do chung ta thay rang, return co chuc nang giu lai gia tri cua bien, va gia
--tri do khong bien mat khi bien ra khoi ham, 

--nhap du lieu tu ban phim
print ("nhap so a: ")
local a = io.read()
print ("so a", a)
------------------
