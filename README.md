git 分支提交描述：

git init 初始化  
git add README.md  
git commit -m "first commit"  
git remote add origin https://github.com/sunwantong/test_pro.git //和远程仓库关联起来  
git push -u origin master  //初次提交加 -u参数  


//非初次提交
git add .  
git commit -m 'test'  
git push origin master//push到远程仓库  

//本地建立分支,并将新的分支同步到远程仓库  
git checkout -b  labelCntBranch  (本地建立新的分支并切换到新的分支，labelCntBranch为新的分支名)  
git push origin labelCntBranch  (和远程仓库同步，并在远程仓库建立labelCntBranch分支,如果该远程分支不存在，则会被新建)  

//提交文件到远程labelCntBranch分支  
git add .  
git commit - 'aa'  
git push origin labelCntBranch
