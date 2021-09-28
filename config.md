# config | git 설정 파일

> 사용자 정보 (commit author) : 커밋을 하기 위해 반드시 필요

```bash
git config --global user.name "닉네임"
git config --global user.email "이메일"
```

> 설정 확인

```bash
git config -l
git config --global -l
git config user.name
```

### system

> 시스템의 모든 사용자와 모든 저장소에 적용(관리자 권한)

```bash
/etc/gitconfig
```

### global

> 현재 사용자에게 적용되는 설정

```bash
~/.gitconfig
```

### local

> 특정 저장소에만 적용되는 설정

```bash
.git/config
```



## `config`

* 기본 에디터 : `vim` => visual studio code로 변경

```bash
$ git config --global core.editor "code --wait"
```



##### 명령어

```bash
visual studio code로 편집기 설정 | git config --global core.editor "code--wait"
```

```bash
vim 창 종료하는 법 | esc+w+q
```



## `.gitignore`

> git으로 관리하지 않을 파일 목록

```bash
# 특정 파일
data.csv
# 특정 폴더
secret/
# 특정 확장자 (*)
*.csv
```

* 일반적인 개발 환경에서 필수적으로 등록하는 예시

  * OS, IDE(eclipse) / Text editor(vs code), 특정 언어나 프레임워크에서 생성되는 파일 

    * ex) 임시파일/실행을 위해서 필요한 파일

    * https://github.com/github/gitignore/blob/master/Java.gitignore

    * https://gitignore.io/ 

      * 예시) `windows`, `java`, `eclipese`

      ```bash
      # Created by https://www.toptal.com/developers/gitignore/api/windows,java,eclipse
      # Edit at https://www.toptal.com/developers/gitignore?templates=windows,java,eclipse
      
      ### Eclipse ###
      .metadata
      bin/
      tmp/
      *.tmp
      *.bak
      *.swp
      *~.nib
      local.properties
      .settings/
      .loadpath
      .recommenders
      
      # External tool builders
      .externalToolBuilders/
      
      # Locally stored "Eclipse launch configurations"
      *.launch
      
      # PyDev specific (Python IDE for Eclipse)
      *.pydevproject
      
      # CDT-specific (C/C++ Development Tooling)
      .cproject
      
      # CDT- autotools
      .autotools
      
      # Java annotation processor (APT)
      .factorypath
      
      # PDT-specific (PHP Development Tools)
      .buildpath
      
      # sbteclipse plugin
      .target
      
      # Tern plugin
      .tern-project
      
      # TeXlipse plugin
      .texlipse
      
      # STS (Spring Tool Suite)
      .springBeans
      
      # Code Recommenders
      .recommenders/
      
      # Annotation Processing
      .apt_generated/
      .apt_generated_test/
      
      # Scala IDE specific (Scala & Java development for Eclipse)
      .cache-main
      .scala_dependencies
      .worksheet
      
      # Uncomment this line if you wish to ignore the project description file.
      # Typically, this file would be tracked if it contains build/dependency configurations:
      #.project
      
      ### Eclipse Patch ###
      # Spring Boot Tooling
      .sts4-cache/
      
      ### Java ###
      # Compiled class file
      *.class
      
      # Log file
      *.log
      
      # BlueJ files
      *.ctxt
      
      # Mobile Tools for Java (J2ME)
      .mtj.tmp/
      
      # Package Files #
      *.jar
      *.war
      *.nar
      *.ear
      *.zip
      *.tar.gz
      *.rar
      
      # virtual machine crash logs, see http://www.java.com/en/download/help/error_hotspot.xml
      hs_err_pid*
      
      ### Windows ###
      # Windows thumbnail cache files
      Thumbs.db
      Thumbs.db:encryptable
      ehthumbs.db
      ehthumbs_vista.db
      
      # Dump file
      *.stackdump
      
      # Folder config file
      [Dd]esktop.ini
      
      # Recycle Bin used on file shares
      $RECYCLE.BIN/
      
      # Windows Installer files
      *.cab
      *.msi
      *.msix
      *.msm
      *.msp
      
      # Windows shortcuts
      *.lnk
      
      # End of https://www.toptal.com/developers/gitignore/api/windows,java,eclipse
      ```

      