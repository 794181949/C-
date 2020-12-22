## 作用
用于中止循环， 只能用于for while， do while， swithch
如果是用于if里面的话，就是需要在for循环里面，然后中止了for 循环

## 用于多重for循环

    int i,j;
    for (i = 0; i < 3; i++){
      for (j = 1; j <4; ++j){
        break;
      printf("good\n");
    }
  }

break只能用于离他最近的循环

## continue
用于跳过本次循环的余下内容，进入判断是否需要进入下次循环

    for (1;2 ;3){
      A;
      B;
      continue;
      C;
    }
    
这时候C语句会被跳过
