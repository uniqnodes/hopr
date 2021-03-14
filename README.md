![alt text](https://cdn-images-1.medium.com/max/308/1*RUlmJOG_Y0KbTkVlA3AFCA@2x.png)

# Hopr Jungfrau Node (ubuntu 18.04)
*(Bu kurulum bir user üzerinde yapılabilir. Başlamak için önce user oluşturun.)*  

`sudo mkdir -m 777 hopr-node`  
`cd hopr-node`  
`sudo apt install -y curl`  
`curl https://raw.githubusercontent.com/hoprnet/hopr-sh/master/setup-hoprd.sh --output setup-hoprd.sh`  
`chmod +x setup-hoprd.sh`  
`./setup-hoprd.sh`  
Do you agree to our Privacy Policy? [y/n]: `y`  
Would you like to run this script? [y/n]: `y`  
What release are you installing? `1.70.8`  
`sudo apt install tmux`  
`tmux`  
`DEBUG=hopr*,libp2p:mplex:stream hoprd --init --rest --admin --adminHost 0.0.0.0` *(bu sadece VPS kurulumu için. diğerleri için https://github.com/hoprnet/hopr-sh sayfasında Running HOPRd başlığına bakın)*  
password: `<BİR ŞİFRE BELİRLEYİN>`  

Tarayıcınızdan `<SERVER-IP>:3000` ile node dashboardınıza ulaşın
