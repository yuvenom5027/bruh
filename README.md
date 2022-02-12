import random
import discord
from dotenv import load_dotenv
load_dotenv()
TOKEN = os.getenv('token')

TOKEN = '?????????????'

client = discord.Client()


@client.event
async def on_ready():
    print('We have logged in as {0.user}'.format(client))
    print('Ready to use')


@client.event
async def on_message(message):
    username = str(message.author).split('#')[0]
    user_message = str(message.content)
    channel = str(message.channel.name)
    print(f'{username}: {user_message}({channel})')

    if message.author == client.user:
        return
    if message.channel.name == 'geral':
        if user_message.lower() == 'hello':
            await message.channel.send(f'hello {username}')
            return
        elif user_message.lower() == 'bye':
            await message.channel.send(f'see you later {username}')
            return
        elif user_message.lower() == '-roll':
            response = f'This is your random number: {random.randrange(100)}'
            await message.channel.send(response)
            return

    if user_message.lower() == '-potato':
        batata1 = 'https://w7.pngwing.com/pngs/320/313/png-transparent-potato-vegetable-tomato-onion-food-potato-food-tomato-onion.png'
        batata2 = 'https://hiperideal.vteximg.com.br/arquivos/ids/167660-1000-1000/27502.jpg'
        batata3 = 'https://www.pngitem.com/pimgs/m/109-1097968_kawaii-potatokawaii-potato-cute-cute-potato-transparent-background.png'
        batata4 = 'https://www.pikpng.com/pngl/m/300-3009374_kawaii-potato-transparent-kawaii-potato-png-clipart.png'
        batata5 = 'https://img2.gratispng.com/20171201/43e/potato-high-quality-png-5a21d44d4dd613.4451836915121664773188.jpg'
        batata6 = ''
        await message.channel.send (random.choice((batata1, batata2, batata3, batata4, batata5, batata6)))
        return

    if user_message.lower() == '-bruh':
        bruh1 = 'https://c.tenor.com/DB-MaLK8iBwAAAAC/bruh-zone-bruh.gif'
        bruh2 = 'https://titterfun.com/api/assets/image/349dzoyzmex1.jpg'
        bruh3 = 'https://i.kym-cdn.com/photos/images/facebook/001/892/610/3bd.png'
        bruh4 = ''
        bruh5 = 'https://i.pinimg.com/originals/66/cf/a2/66cfa282a682753931905b8cce9d4f07.jpg'
        bruh6 = 'https://i.pinimg.com/originals/39/78/86/3978862a1005c07a18b9d032cc494ef9.jpg'
        bruh7 = 'https://www.kindpng.com/picc/m/16-165695_charlotte-anime-meme-face-hd-png-download.png'
        await message.channel.send (random.choice((bruh1, bruh2, bruh3, bruh4, bruh5, bruh6, bruh7)))
        return

    if user_message.lower() == '-stare':
        stare1 = 'https://i.pinimg.com/474x/b6/bc/dc/b6bcdcce0972190f83ff8d511f352bb8.jpg'
        stare2 = 'https://c.tenor.com/OGYkjgAqocgAAAAC/anime-stare.gif'
        stare3 = 'https://c.tenor.com/YZqZDBRGYogAAAAC/anime-okay-then.gif'
        stare4 = 'https://i.pinimg.com/474x/63/12/61/6312617f6e03312e163569d182ce70bd.jpg'
        stare5 = 'https://i1.wp.com/animediet.net/wp-content/uploads/2011/07/moritasan2.jpg'
        stare6 = 'https://external-preview.redd.it/jBIgtkj2ST5uhgE_mYAgiu3-lRllNamhASAsFNBi5sk.jpg?auto=webp&s=8c96887ef518788959e1eb132ccf7de4c3d27a7b'
        stare7 = 'https://c.tenor.com/-htQlAzVwKcAAAAC/anime-blinking.gif'
        stare8 = 'http://pm1.narvii.com/6660/4cbd56c8366b9d7c9470e3fa4179dddb0a07f713_00.jpg'
        await message.channel.send (random.choice((stare1, stare2, stare3, stare4, stare5, stare6, stare7, stare8)))
        return

    if user_message.lower() == '-random':
        random1 = 'https://i.kym-cdn.com/photos/images/newsfeed/002/031/703/b68.gif'
        random2 = 'https://media.tenor.com/images/5a692abd85c6705a1542fe0c6542d5fe/tenor.png'
        random3 = 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQN2uwXQ1vBIHH9DyT2M4AFvv6BdV9vIPk4bw&usqp=CAU'
        random4 = 'https://media.tenor.com/images/0389e997893bebe17233cfcbfd456af4/tenor.png'
        random5 = 'https://i.pinimg.com/474x/1e/8f/3e/1e8f3e36e6fa13007caa610295d5684f.jpg'
        random6 = 'https://i.pinimg.com/originals/56/65/4e/56654eb38f6ed08f81ebd395e98197ac.gif'
        random7 = 'https://i.pinimg.com/236x/94/47/c6/9447c6972019def331675628061c1707.jpg'
        random8 = 'https://c.tenor.com/lve6oowtLt4AAAAd/hideri-kanzaki-blend-s.gif'
        random9 = 'https://i.pinimg.com/474x/93/cb/3c/93cb3cce9fbc121470b61d61ce111933.jpg'
        random10 = 'https://i.ytimg.com/vi/g6ry3mQEbdY/maxresdefault.jpg'
        random11 = 'https://tiermaker.com/images/templates/anime-best-masterpiece-803702/8037021612325044.png'
        random12 = 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTyvEqV9jHGObGU9pLnm_dRB_b0TnD2y2lk6w&usqp=CAU'
        random13 = 'https://animemotivation.com/wp-content/uploads/2018/07/Kyoko-smug-face-yuru-yuri.gif'
        random14 = 'https://i.pinimg.com/originals/ac/ab/86/acab86fdc6a3aa354e2bf5ee774ba3a3.png'
        random15 = 'https://i.pinimg.com/originals/db/18/79/db1879076d892104dbf485f16e6b134f.gif'
        random16 = 'https://i.pinimg.com/550x/c8/48/a6/c848a6ed9d2eba3f047b5bb5956fd7f9.jpg'
        await message.channel.send (random.choice(((random1, random2, random3, random4, random5, random6, random7, random8, random9, random10, random11, random12, random13, random14, random15, random16))))
        return

    if user_message.lower() == '-help':
        await message.channel.send('use -potato to get random potato pics, use -bruh for random bruh pics, use -stare to get random anime character staring at you and finally use -random to get some random pics' )
client.run(TOKEN)
