1.Warmup-1 > sleepIn
public boolean sleepIn(boolean weekday, boolean vacation) {
  if (!weekday || vacation) {
    return true;
  }
  
  return false;
}

2.Warmup-1 > monkeyTrouble
public boolean monkeyTrouble(boolean aSmile, boolean bSmile) {
  if(aSmile==bSmile)
 {
   return true;
 }
 return false;
}

3.public int sumDouble(int a, int b) {
  if(a==b)
  {
    return(2*(a+b));
  }
   return(a+b);
}
4.public int diff21(int n) {
  if(n<=21)
  {
  return(21-n);
}
return(2*(n-21));
}
5.
5.public int diff21(int n) {
  if(n<=21)
  {
  return(21-n);
}
return(2*(n-21));
}
6.public boolean parrotTrouble(boolean talking, int hour) {
  if(talking==true && (hour<7||hour>20))
  {
  return true;
}
return false;
}
7.public boolean makes10(int a, int b) {
  if((a==10||b==10) || (a+b==10))
  {
    return true;
  }
  return false;
}
8.public boolean nearHundred(int n) {
  return ((Math.abs(100 - n) <= 10) || (Math.abs(200 - n) <= 10));
}
9.public boolean posNeg(int a, int b, boolean negative) {
  if(((a<0&&b>0 || a>0&&b<0) && (negative==false)) || ((a<0&&b<0)&&(negative==true)))
  {
    return true;
  }
  return false;
}
10.public String notString(String str) {
   if (str.length() >= 3 && str.substring(0, 3).equals("not")) {
    return str;
  }
  
  return "not " + str;
}

11.public String missingChar(String str, int n) {
   String front = str.substring(0, n);
  String back = str.substring(n+1, str.length());
  
  return front + back;
}

11.public String frontBack(String str) {
  if(str.length()<=1)return str;
  String mid=str.substring(1,str.length()-1);
  return str.charAt(str.length()-1) + mid + str.charAt(0);
  
}
12.public boolean or35(int n) {
  if(n%3==0 || n%5==0)
  {return true;
  }
  return false;
}
13.public String front22(String str) {
  String front;
  int a=2;
  if(str.length()<a)
 { return str+str+str;}
  else
  {front=str.substring(0,a);
  return front+str+front;}
}
14.public boolean startHi(String str) {
   if(str.length()<2) return false;
  String front=str.substring(0,2);
  if(front.equals("hi"))
 
  {return true;
}
return false;}
14.public boolean icyHot(int temp1, int temp2) {
  if(temp1<0&&temp2>100 || temp2<0&&temp1>100){
  return true;
}
return false;}
15.public boolean in1020(int a, int b) {
  if((a >= 10 && a <= 20) || (b >= 10 && b <= 20))
  {
    return true;
  }return false;
}
16.public boolean hasTeen(int a, int b, int c) {
  if((a>=13&&a<=19) || (b>=13&&b<=19) ||(c>=13&&c<=19))
  {
    return true;
    
  }return false;
}
17.public boolean loneTeen(int a, int b) {
  Boolean teen1=(a>=13&&a<=19);
  Boolean teen2=(b>=13&&b<=19);
   if((teen1 && !teen2) || (!teen1 && teen2)){
   
    return true;
    
  }return false;
}
18.public String delDel(String str) {
  if (str.length()>=4 && str.substring(1, 4).equals("del")) {
    return str.substring(0, 1) + str.substring(4);
  }
  return str;
}
19.public boolean mixStart(String str) {
  if((str.length()>=3) && (str.substring(1,3).equals("ix"))){
  return true;}
  return false;
}
20.public String startOz(String str) {
   String result = "";
  
  if (str.length() >= 1 && str.charAt(0)=='o') {
    result = result + str.charAt(0);
  }
  
  if (str.length() >= 2 && str.charAt(1)=='z') {
    result = result + str.charAt(1);
  }
  
  return result;
}

21.public int intMax(int a, int b, int c) {
  if(a>b && a>c) return a;
  else if(b>a && b>c) return b;
  else return c;
}
22.public int close10(int a, int b) {
  if(Math.abs(a-10)<Math.abs(b-10))
  {return a;
}
  if(Math.abs(b-10)<Math.abs(a-10))
  {return b;
}return 0;
}
23.public boolean in3050(int a, int b) {
  if((a>=30&&a<=40)&&(b>=30&&b<=40)) return true;
  if((a>=40&&a<=50)&&(b>=40&&b<=50)) return true;
  return false;
  

}
24.public int max1020(int a, int b) {
  if (b > a) {
    int temp = a;
    a = b;
    b = 27;
temp;
  }
  if (a >= 10 && a <= 20) return a;
  if (b >= 10 && b <= 20) return b;
  return 0;
}
25.public boolean stringE(String str) {
   int count = 0;

  for (int i=0; i<str.length(); i++) {
    if (str.charAt(i) == 'e') count++;
  }

  return (count >= 1 && count <= 3);
}
26.public boolean lastDigit(int a, int b) {
  if(a%10==b%10) {
    return true;}
    return false;
  }

27.public String endUp(String str) {
  if(str.length() <= 3) return str.toUpperCase();
  int n=(str.length()-3);
  String front=str.substring(0,n);
  String back=str.substring(n);
  return front+back.toUpperCase();
}
28public String endUp(String str) {
  if(str.length() <= 3) return str.toUpperCase();
  int n=(str.length()-3);
  String front=str.substring(0,n);
  String back=str.substring(n);
  return front+back.toUpperCase();
}

29.public String everyNth(String str, int n) {
  String result = "";
  
  // Look at every nth char
  for (int i=0; i<str.length(); i = i + n) {
    result = result + str.charAt(i);
  }
  return result;
}
