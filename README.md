# divide-big-num
Python code to divide big numbers 



####CODE####
import math
def chiahaisolon(sobichia, sochia):

	a = "";
	b = 0;
	temp = ord(sobichia[b]) - ord('0');
	while (temp < sochia):
		temp = (temp * 10 + ord(sobichia[b + 1]) - ord('0'));
		b += 1;
	
	b += 1;

	while ((len(sobichia)) > b):
		
		a += chr(math.floor(temp // sochia) + ord('0'));
		
		temp = ((temp % sochia) * 10 + ord(sobichia[b]) - ord('0'));
		b += 1;

	a += chr(math.floor(temp // sochia) + ord('0'));
	

	if (len(a) == 0):
		return "0";
	
	return a;

sobichia = "1248163264128256512";
sochia = 125;
print(chiahaisolon(sobichia, sochia));





### OR YOU CAN DOWNLOAD ###
print(chiahaisolon(sobichia, sochia));
