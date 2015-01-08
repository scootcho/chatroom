##chatroom client

tutorial: http://code.tutsplus.com/tutorials/how-to-use-faye-as-a-real-time-push-server-in-rails--net-22600

working using Faye. Switching over to Public_private gem. Need couple of tweaks for it to work.

start the thin server:

`rackup private_pub.ru -s thin -E production`

localhost:3000/login

sign in with a username

go to 

localhost:3000/chatroom for chat.

---

##TODO

currenlty the private message will only get one word. Example. "@scoot hey there wassup" will only send "hey".

Fix: in chats_controller 'if recipient = params[:message].match(/@(\w+) (.+)/)'

messages are not sending/displaying using public_private
