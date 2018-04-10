#include <stdbool.h>
#include <stdint.h>
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include <windows.h>
int main(int argc, char ** argv) {
    int32_t v1;
    char * str = (char *)v1;
    ___main();
    SetConsoleTitleA("IP Changer by Heena");
    puts("Enter your choice: ");
    puts("1.Static\n2.DHCP");
    int32_t v2;
    scanf("%d", &v2);
    switch (v2) {
        default: {
            puts("Wrong Input");
            break;
        }
        case 2: {
            system("cmd.exe /c netsh interface ip set address \"Local Area Connection\" dhcp");
            _sleep(4);
            system("cmd.exe /c netsh interface ip set dns \"Local Area Connection\" dhcp");
            puts("Done!");
            break;
        }
        case 1: {
            str = (char *)0x2e646d63;
            int32_t v3;
            int32_t v4;
            int32_t v5;
            memcpy((char *)&v5, (char *)&v4, (int32_t)&v3);
            printf("Enter suffix: ");
            int32_t str2;
            scanf("%s", &str2);
            strcat((char *)&str, (char *)&str2);
            int32_t str3;
            strcpy((char *)&str3, (char *)&str);
            strlen((char *)&str3);
            system((char *)&str3);
            _sleep(4);
            system("cmd.exe /c netsh interface ip set dns \"Local Area Connection\" static 192.168.88.1");
            puts("Done!")
            break;
        }
     }
    _getch();
    return 0;
}
