--bai 1: tinh tong cac so tu 1 den N
function tinhtongN(n)
 local tong = 0
 for i = 1, n, 1 do
   tong = tong + i
 end
 return tong
end
ketquabai1 = tinhtongN(10)
print ("tong tu 1 den N la: ", ketquabai1)
------------------------------------
--bai 2: kiem tra so nguyen to
function songuyento(n)
  if n > 1 then
    local ketquabai2 = 0
    for i = 2, n - 1, 1 do
      ketquabai2 = n % i
      if ketquabai2 == 0 then
        print ("Day khong phai la so nguyen to")
        return
      end
    end
    print ("Day la so nguyen to")
  else 
    print ("Day khong phai la so nguyen to")
  end    
end
songuyento(4)
------------------------------------
--bai 3: tinh giai thua cua 1 so nguyen duong
function tinhgiaithua(n)
  if n > 0 then
    local ketquabai3 = 1
      for i = n, 1, -1 do
        ketquabai3 = ketquabai3 * i
      end
      print(ketquabai3)
    else 
      print ("Day khong phai la so nguyen duong")
  end
end
tinhgiaithua(5)
------------------------------------
