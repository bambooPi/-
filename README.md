# -
一些算法的集锦
素数筛
void isp()
  {
      memset(p,0,sizeof(p));
      p[0]=1;p[1]=1;p[2]=0;
      for(int i=0;i<10000;i++)
      {
          if(p[i])
              continue;
          for(int j=i;j*i<10000;j++)
          {
              p[i*j]=1;
          }
          prim[len++]=i;
      }
  
  }
