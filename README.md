# VAMP-SQUAD
#include <stdio.h>
#include<string.h>
int main()
{
    char boy[10],girl[10];
    int len1,len2,i,j,len=0,blen=0,glen=0;
    printf("enter the boy name:\n");
    scanf("%s",boy);
    printf("enter girl name:\n");
    scanf("%s",girl);
    len1=strlen(boy);
    len2=strlen(girl);
    for(i=0;i<len1;i++)
      {
          for(j=0;j<len2;j++)
          {
              if(boy[i]==girl[j])
              {
                  boy[i]='*';
                 girl[j]='*';
                 
               }
              
          }
      }
     printf("%s %s",boy,girl);

for(i=0;i<len1;i++)
{ 
    if(boy[i]=='*')
       { 
       continue;
          
        }
     else
     {
         blen++;
     }
}
for(i=0;i<len2;i++)
{ 
    if(girl[i]=='*')
       { 
       continue;
          
        }
     else
     {
         glen++;
      }
    
}
    len=blen+glen;
    printf("%d",len);
}
