# final 2024.01.12
## a.h
```c
typedef unsigned char c;typedef unsigned long u;u Q=96;
#define $(a,b) if(a)b;else
#define ax (256>x)
#define xi (nx>i?sx[i]:0)
#define i(n,e) {int $n=n;int i=0;for(;i<$n;++i){e;}}
#define _(e) ({e;})
#define _u(f,e,x...) u f(x){return({e;});}
#define nx sx[-1]
#define sx ((c*)x)
#define x(a,e) _(u x=a;e)
#define y(a,e) _(u y=a;e)
#define f(g,e) _u(g,e,u x)
#define F(g,e) _u(g,e,u f,u x)
#define G(g,e) _u(g,e,u f,u x,u y)
#define us(f,e) _u(f,e,c*s)
#define Q(e) if(Q==(e))return Q;
#define Qr(e) if(e){return err((u)__func__,(u)"rank");}
#define Qz(e) if(e){return err((u)__func__,(u)"nyi");}
#define sr x(r,sx)
#define ri sr[i]

#define af x(f,ax)
#define nf x(f,nx)
#define sf x(f,sx)
#define fi x(f,xi)
```
## a.c
```c
#include"a.h"//fF[+-!#,@] atom/vector 1byteint 1bytetoken  no(memmanage parser tokens ..) clang-13 -Os -oa a.c -w 
#define r(n,e) _(u r=a(n);i(n,ri=e)r)
f(w,write(1,ax?(u)&x:x,ax?1:strlen(x)))
c b[12];
f(si,sprintf(b,"%d ",128>x?x:x-256);b)
f(wi,w(si(x)))
f(w_,$(ax,wi(x))i(nx,wi(xi))w(10))

F(err,w(f);w(58);w(x);w(10);96)
G(m,(u)memcpy((void*)x,(void*)y,f))
f(a,c*s=malloc(x+1);*s++=x;(u)s)
f(foo,Qz(1)0)
f(sub,ax?(c)-x:r(nx,-xi))
f(ind,Qr(!ax)r(x,i))
f(cnt,Qr(ax)nx)
f(cat,Qr(!ax)r(1,x))
F(Add,ax?af?f+x:Add(x,f):r(nx,(af?f:fi)+xi))
F(Sub,Add(f,sub(x)))
F(Ind,Qr(!f)r(nx,xi%f))
F(Cnt,Qr(!af)r(f,ax?x:xi))
F(Cat,f=af?cat(f):f;x=ax?cat(x):x;u r=a(nf+nx);m(nx,r+nf,x);m(nf,r,f))
F(At,Qr(af)ax?sf[x]:r(nx,sf[xi]))f(at,At(x,0))
char*V=" +-!#,@";u(*f[])()={0,foo,sub,ind,cnt,cat,at},(*F[])()={0,Add,Sub,Ind,Cnt,Cat,At},U[26];
f(v,(strchr(V,x)?:V)-V)
f(n,10>x-48?x-48:U[x-97])
us(e,u i=*s++;v(i)?x(e(s),Q(x)f[v(i)](x)):x(n(i),*s?y(e(s+1),Q(y)F[v(*s)](x,y)):x))
int main(){char s[99];while(1)if(w(32),s[read(0,s,99)-1]=0,*s)w_(e(s));}
```
# 2024.01.10
## a.h
```c
typedef unsigned long u;
#define _u(f,e,x...) u f(x){return _(e);}
#define ax (10>x)
#define nx sx[-1]
#define sx ((char*)x)
#define xi sx[i]
#define _(e) ({e;})
#define r(a,e) _(u r=a;e;r)
#define x(a,e) _(u x=a;e)
#define y(a,e) _(u y=a;e)
#define i(n,e) {int $n=n;int i=0;for(;i<$n;++i){e;}}
#define f(f,e) _u(f,e,u x)
#define F(f,e) _u(f,e,u x,u y)
#define G(g,e) _u(g,e,u f,u x,u y)
#define us(f,e) _u(f,e,char*s)
#define Q(e) if(96==(e))return 96;
#define Qr(e) if(e){return err((u)__func__,(u)"rank");}
#define Qz(e) if(e){return err((u)__func__,(u)"todo");}
#define ri sr[i]
#define yi x(y,xi)
#define nr x(r,nx)
#define ny x(y,nx)
#define sr x(r,sx)
#define sy x(y,sx)
#define ay x(y,ax)

```
## a.c
```c
#include"a.h"//cc -Os -oa a.c -w
F(w_,write(1,y,x))f(w,127>x?w_(1,(u)&x):w_(strlen(x),x))F(err,w(x);w(58);w(y);w(10);96)f(qz,Qz(1)0)
G(m,(u)memcpy((void*)x,(void*)y,f))
f(a,char*s=malloc(x+1);*s++=x;(u)s)
f(ind,Qr(!ax)x=a(x);i(nx,xi=i)x)
f(cat,Qr(!ax)u r=a(1);*sr=x;r)
F(Cat,x=ax?cat(x):x;y=ay?cat(y):y;u r=a(nx+ny);m(ny,r+nx,y);m(nx,r,x))
f(at,Qr(ax)*sx)
F(At,Qr(ax||!ay)sx[y])
f(cnt,Qr(ax)nx)
F(Cnt,Qr(!ax||ay)x=a(x);m(nx,x,y))
F(Add,ax?ay?x+y:Add(y,x):r(a(ny),i(nr,ri=(ax?x:xi)+yi)))
u(*f[])()={0,qz,ind,cnt,cat,at},(*F[])()={0,Add,qz,Cnt,Cat,At};
u U[26];f(n,10>x-48?x-48:U[x-97])
char*V=" +!#,@";f(v,(strchr(V,x)?:V)-V)
us(e,u i=*s++;v(i)?x(e(s),Q(x)f[v(i)](x)):x(n(i),*s?y(e(s+1),Q(y)F[v(*s)](x,y)):x))
us(ws,u x=*s?e(s):0;Q(x)ax?w(48+x):_(i(nx,w(48+xi);w(32))0);w(10))
int main(){char s[99];while(1)w(32),s[read(0,s,99)-1]=0,ws(s);}

char *kinit(){char s[99];return s;}
```
# initial 2024.01.10
```c
typedef char c;typedef unsigned long(*_)(),u;
#define _(e) ({e;})
#define s(f,e,x...) c*f(x){return _(e);}
#define u(f,e,x...) u f(x){return _(e);}
#define I(n,e) {int $n=n;int i=0;for(;i<$n;++i){e;}}
#define f(f,e) u(f,e,u x)
#define F(f,e) u(f,e,u x,u y)
#define sr ((c*)r)
#define sx ((c*)x)
#define sy ((c*)y)
#define nr sr[-1]
#define nx sx[-1]
#define ny sy[-1]
#define rc sr[i]
#define xc sx[i]
#define yc sy[i]
#define ax (10>x)
#define ay (10>y)
#define oo w_(3,"oo\n")
#define r(a,e) _(u r=a;e;r)
u(m,(u)memcpy((void*)x,(void*)y,n),u n,u x,u y)u(w_,write(1,s,n),u n,c*s)f(w,w_(1,&x))
f(a,c*s=malloc(x+1);*s++=x;(u)s)f(ind,x=a(x);I(nx,xc=i)x)
f(cat,u r=a(1);*sr=x;r)F(Cat,x=ax?cat(x):x;y=ay?cat(y):y;u r=a(nx+ny);m(ny,r+nx,y);m(ny,r,x))
f(at,*sx)F(At,sx[y])f(cnt,nx)F(Cnt,x=a(x);m(nx,x,y))
F(Add,ax?ay?x+y:Add(y,x):r(a(ny),I(nr,rc=(ax?x:xc)+yc)))
f(q,0)_ f[]={0,q,ind,cnt,cat,at},F[]={0,Add,q,Cnt,Cat,At};
u U[26];f(n,10>x-48?x-48:U[x-97])c*V=" +!#,@";f(v,(strchr(V,x)?:V)-V)
u(e,c i=*s++;v(i)?f[v(i)](e(s)):*s?F[v(*s)](n(i),e(s+1)):n(i),c*s)
u(ws,u x=*s?e(s):0;ax?w(48+x):_(I(nx,w(48+xc);w(32))0);w(10),c*s)
int main(){c s[99];while(1)w(32),s[read(0,s,99)-1]=0,ws(s);}
```