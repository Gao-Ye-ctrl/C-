# C-
# 新手学习C语言的一个一个代码






##############
#1.小小恶搞关机程序
int main() {
	char input[200] = { 0 };
	system("shutdown -s -t 60");
again:
	
		printf("屏幕前的大笨猪，你的电脑将要在1分钟内关机。如果输入：王春燕喜欢高志伟。就取消关机\n");
		scanf("%s", input);
		if (strcmp(input, "王春燕喜欢高志伟") == 0)
		{
			system("shutdown -a");
			printf("关机已取消\n");
			
		}
		else {
			goto again;
		}


	return 0;
}

