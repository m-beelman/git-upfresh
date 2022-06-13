# git upfresh - Conference session preparation

## Topics for the confrence talk

* git stash (possible with link to stashing partially staged changes) (<https://github.blog/2022-01-24-highlights-from-git-2-35/>)
* git sparse checkout (<https://github.blog/2021-11-15-highlights-from-git-2-34/>)
* ort merge algorithm
* replace a single commit (amend) with fixup

        
   1980 marko     20   0  172576   4364   3764 S   0,3   0,1   0:02.56 ibus-engine-sim                                                                                                                             
   2233 marko     20   0  632920  73180  32860 S   0,3   0,9  10:05.21 Xwayland                                                                                                                                    
 108730 marko     20   0 2475432 129116  82420 S   0,3   1,6   0:06.68 Isolated Web Co                                                                                                                             
 132635 marko     20   0 2512188 161664  79776 S   0,3   2,0   0:29.68 Isolated Web Co                                                                                                                     top - 21:34:30 up 12 days, 10:49,  1 user,  load average: 0,92, 0,55, 0,47
Tasks: 318 gesamt,   1 laufend, 317 schlafend,   0 gestoppt,   0 Zombie
%CPU(s): 12,3 us,  2,7 sy,  0,0 ni, 84,7 id,  0,1 wa,  0,0 hi,  0,2 si,  0,0 st
MiB Spch :   7832,2 gesamt,    849,0 frei,   4000,8 belegt,   2982,4 Puff/Cache
MiB Swap:   2048,0 gesamt,   1616,4 frei,    431,6 belegt.   2869,2 verfü Spch 

    PID USER      PR  NI    VIRT    RES    SHR S  %CPU  %MEM     ZEIT+ BEFEHL                                                                                                                              
  17142 marko     20   0   12,4g 511408 160444 S  24,4   6,4  83:57.97 firefox                                                                                                                             
 148947 marko     20   0 3304728 552000  98852 S  18,8   6,9   4:59.23 Isolated Web Co                                                                                                                     
   1925 marko     20   0 1410616 314008  35248 S   7,3   3,9  22:57.38 snap-store                                                                                                                          
   1559 marko     20   0 5337372 281828  79300 S   4,0   3,5  24:41.55 gnome-shell                                                                                                                         
 155716 marko     20   0 2792728 221108 100888 S   1,0   2,8  25:56.28 Isolated Web Co                                                                                                                     
 165010 marko     20   0 2459596 110368  84140 S   1,0   1,4   0:00.76 Isolated Web Co                                                                                                                     
  19758 marko     20   0 2565864 202480  54400 S   0,7   2,5   1:03.89 WebExtensions                                                                                                                       
  51704 root      20   0 1427524  20144   8640 S   0,7   0,3   0:41.53 containerd                                                                                                                          
     13 root      20   0       0      0      0 I   0,3   0,0   0:37.25 rcu_sched                                                                                                                           
    223 root      20   0       0      0      0 S   0,3   0,0   0:11.14 jbd2/sda2-8                                                                                                                         
    383 root     -51   0       0      0      0 S   0,3   0,0   2:15.43 irq/127-iwlwifi                                                                                                                     
    427 systemd+  20   0   14776   4696   3908 S   0,3   0,1   1:20.35 systemd-oomd                                                                                                                        
  19359 marko     20   0 2459936 122872  66848 S   0,3   1,5   0:23.26 Privileged Cont                                                                                                                     
  20237 marko     20   0  573476  46800  33032 S   0,3   0,6   1:31.18 gnome-terminal-                                                                                                                     
 147076 marko     20   0 2781044 262836  86168 S   0,3   3,3   1:00.98 Isolated Web Co                                                                                                                     
 154539 marko     20   0   22156   4372   3368 R   0,3   0,1   1:21.58 top                                                                                                                                 
 165149 root      20   0       0      0      0 I   0,3   0,0   0:00.03 kworker/1:4-events                                                                                                                  
      1 root      20   0  176184  11456   6376 S   0,0   0,1   0:10.67 systemd                                                                                                                             
      2 root      20   0       0      0      0 S   0,0   0,0   0:00.04 kthreadd                                                                                                                            
      3 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 rcu_gp                                                                                                                              
      4 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 rcu_par_gp                                                                                                                          
      6 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/0:0H-events_highpri                                                                                                         
      9 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 mm_percpu_wq                                                                                                                        
     10 root      20   0       0      0      0 S   0,0   0,0   0:00.00 rcu_tasks_rude_                                                                                                                     
     11 root      20   0       0      0      0 S   0,0   0,0   0:00.00 rcu_tasks_trace                                                                                                                     
     12 root      20   0       0      0      0 S   0,0   0,0   0:02.00 ksoftirqd/0                                                                                                                         
     14 root      rt   0       0      0      0 S   0,0   0,0   0:00.24 migration/0                                                                                                                         
     15 root     -51   0       0      0      0 S   0,0   0,0   0:00.00 idle_inject/0                                                                                                                       
     16 root      20   0       0      0      0 S   0,0   0,0   0:00.00 cpuhp/0                                                                                                                             
     17 root      20   0       0      0      0 S   0,0   0,0   0:00.00 cpuhp/1                                                                                                                             
     18 root     -51   0       0      0      0 S   0,0   0,0   0:00.00 idle_inject/1                                                                                                                       
     19 root      rt   0       0      0      0 S   0,0   0,0   0:00.39 migration/1                                                                                                                         
     20 root      20   0       0      0      0 S   0,0   0,0   3:05.85 ksoftirqd/1                                                                                                                         
     22 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/1:0H-events_highpri                                                                                                         
     23 root      20   0       0      0      0 S   0,0   0,0   0:00.00 cpuhp/2                                                                                                                             
     24 root     -51   0       0      0      0 S   0,0   0,0   0:00.00 idle_inject/2                                                                                                                       
     25 root      rt   0       0      0      0 S   0,0   0,0   0:00.39 migration/2                                                                                                                         
     26 root      20   0       0      0      0 S   0,0   0,0   0:02.56 ksoftirqd/2                                                                                                                         
     28 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/2:0H-events_highpri                                                                                                         
     29 root      20   0       0      0      0 S   0,0   0,0   0:00.00 cpuhp/3                                                                                                                             
     30 root     -51   0       0      0      0 S   0,0   0,0   0:00.00 idle_inject/3                                                                                                                       
     31 root      rt   0       0      0      0 S   0,0   0,0   0:00.39 migration/3                                                                                                                         
     32 root      20   0       0      0      0 S   0,0   0,0   0:01.90 ksoftirqd/3                                                                                                                         
     34 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/3:0H-events_highpri                                                                                                         
     35 root      20   0       0      0      0 S   0,0   0,0   0:00.00 kdevtmpfs                                                                                                                           
     36 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 netns                                                                                                                               
marko@hp-lx:~/projects/swcoe-craft-assess-automation$ cd ..
marko@hp-lx:~/projects$ mkdir git
marko@hp-lx:~/projects$ cd gti
bash: cd: gti: Datei oder Verzeichnis nicht gefunden
marko@hp-lx:~/projects$ cd git/
marko@hp-lx:~/projects/git$ git init .
Hinweis: Als Name für den initialen Branch wurde 'master' benutzt. Dieser
Hinweis: Standard-Branchname kann sich ändern. Um den Namen des initialen Branches
Hinweis: zu konfigurieren, der in allen neuen Repositories verwendet werden soll und
Hinweis: um diese Warnung zu unterdrücken, führen Sie aus:
Hinweis: 
Hinweis: 	git config --global init.defaultBranch <Name>
Hinweis: 
Hinweis: Häufig gewählte Namen statt 'master' sind 'main', 'trunk' und
Hinweis: 'development'. Der gerade erstellte Branch kann mit diesem Befehl
Hinweis: umbenannt werden:
Hinweis: 
Hinweis: 	git branch -m <Name>
Leeres Git-Repository in /home/marko/projects/git/.git/ initialisiert
marko@hp-lx:~/projects/git$ git config --global init.defaultBranch main
marko@hp-lx:~/projects/git$ git branch -m main
marko@hp-lx:~/projects/git$ git status
Auf Branch main

Noch keine Commits

nichts zu committen (erstellen/kopieren Sie Dateien und benutzen
Sie "git add" zum Versionieren)
marko@hp-lx:~/projects/git$ ls
marko@hp-lx:~/projects/git$ echo "Hello World!" >> hello.txt
marko@hp-lx:~/projects/git$ git add hello.txt 
marko@hp-lx:~/projects/git$ git commit -am "One" 
Identität des Autors unbekannt

*** Bitte geben Sie an, wer Sie sind.

Führen Sie

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

aus, um das als Ihre standardmäßige Identität zu setzen.
Lassen Sie die Option "--global" weg, um die Identität nur
für dieses Repository zu setzen.

fatal: Konnte die E-Mail-Adresse nicht automatisch erkennen ('marko@hp-lx.(none)' erhalten)
marko@hp-lx:~/projects/git$ git config --global user.email "marko.beelmann@philips.com"
marko@hp-lx:~/projects/git$ git config --global user.email "marko.beelmann@gmail.com"
marko@hp-lx:~/projects/git$ git config --global user.user "Beelmann, Marko"
marko@hp-lx:~/projects/git$ git commit -am "One" 
[main (Root-Commit) c30cc6c] One
 1 file changed, 1 insertion(+)
 create mode 100644 hello.txt
marko@hp-lx:~/projects/git$ echo "Hello World" >> hello.txt && git commit -am "Two"
[main 5776981] Two
 1 file changed, 1 insertion(+)
marko@hp-lx:~/projects/git$ echo "Hello World" >> hello.txt && git commit -am "Three"
[main 6e1589f] Three
 1 file changed, 1 insertion(+)
marko@hp-lx:~/projects/git$ echo "Hello World" >> hello.txt && git commit -am "Four"
[main a667860] Four
 1 file changed, 1 insertion(+)
marko@hp-lx:~/projects/git$ echo "Hello World" >> hello.txt && git commit -am "Five"
[main 71e2b03] Five
 1 file changed, 1 insertion(+)
marko@hp-lx:~/projects/git$ ls ßla
ls: Zugriff auf 'ßla' nicht möglich: Datei oder Verzeichnis nicht gefunden
marko@hp-lx:~/projects/git$ ls -la
insgesamt 16
drwxrwxr-x 3 marko marko 4096 Jun 12 11:24 .
drwxrwxr-x 5 marko marko 4096 Jun 12 11:22 ..
drwxrwxr-x 8 marko marko 4096 Jun 12 11:27 .git
-rw-rw-r-- 1 marko marko   61 Jun 12 11:27 hello.txt
marko@hp-lx:~/projects/git$ git log
commit 71e2b03b4de89d975c654b972f7b33fd8d013759 (HEAD -> main)
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:29 2022 +0200

    Five

commit a66786029adf1136d5dd516d1c93f93a6f99bd0b
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:21 2022 +0200

    Four

commit 6e1589f123213f9d93b09d39c565f51d51fcf434
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:17 2022 +0200

    Three

commit 57769812c319524efaa96a8b9985a0c714061c09
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:12 2022 +0200

    Two

commit c30cc6c8750a50dfe0a15d529c400f45513637f7
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:26:25 2022 +0200

    One
marko@hp-lx:~/projects/git$ git commit --fixup=amend:Tree
fatal: Konnte Commit Tree nicht nachschlagen
marko@hp-lx:~/projects/git$ git commit --fixup=amend:Three
fatal: Konnte Commit Three nicht nachschlagen
marko@hp-lx:~/projects/git$ git commit --fixup=amend:6e158
[main d320976] amend! Three
marko@hp-lx:~/projects/git$ git log
commit d3209763df49f035a65dee55d2daba3d0713d1b4 (HEAD -> main)
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:33:24 2022 +0200

    amend! Three
    
    Three

commit 71e2b03b4de89d975c654b972f7b33fd8d013759
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:29 2022 +0200

    Five

commit a66786029adf1136d5dd516d1c93f93a6f99bd0b
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:21 2022 +0200

    Four

commit 6e1589f123213f9d93b09d39c565f51d51fcf434
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:17 2022 +0200

    Three

commit 57769812c319524efaa96a8b9985a0c714061c09
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:12 2022 +0200

    Two

commit c30cc6c8750a50dfe0a15d529c400f45513637f7
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:26:25 2022 +0200

    One
marko@hp-lx:~/projects/git$ git rebase -i One --autosquash
fatal: Ungültiger Upstream 'One'
marko@hp-lx:~/projects/git$ git rebase -i c30cc --autosquash
Erfolgreich Rebase ausgeführt und refs/heads/main aktualisiert.
marko@hp-lx:~/projects/git$ git log
commit 14bcd75a115b181ab1541904ba929c4cac034c35 (HEAD -> main)
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:29 2022 +0200

    Five

commit 513bc989cb28d51ec3aa06701baa24d3442c2eff
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:21 2022 +0200

    Four

commit c73bdb9a6ac122b778f5de40ad3a80e875ddcb1c
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:17 2022 +0200

    Three

commit 57769812c319524efaa96a8b9985a0c714061c09
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:12 2022 +0200

    Two

commit c30cc6c8750a50dfe0a15d529c400f45513637f7
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:26:25 2022 +0200

    One
marko@hp-lx:~/projects/git$ vim hello.txt 
marko@hp-lx:~/projects/git$ git commit -a --fixup=amend:c73bd
[main d5c2136] amend! Three
 1 file changed, 1 insertion(+), 1 deletion(-)
marko@hp-lx:~/projects/git$ git log
commit d5c2136801551838a307dcc631689d803b71d9d5 (HEAD -> main)
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:35:40 2022 +0200

    amend! Three
    
    Three

commit 14bcd75a115b181ab1541904ba929c4cac034c35
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:29 2022 +0200

    Five

commit 513bc989cb28d51ec3aa06701baa24d3442c2eff
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:21 2022 +0200

    Four

commit c73bdb9a6ac122b778f5de40ad3a80e875ddcb1c
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:17 2022 +0200

    Three

commit 57769812c319524efaa96a8b9985a0c714061c09
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:12 2022 +0200

    Two

commit c30cc6c8750a50dfe0a15d529c400f45513637f7
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:26:25 2022 +0200

    One
marko@hp-lx:~/projects/git$ git rebase -i c73bdb9 --autosquash
Erfolgreich Rebase ausgeführt und refs/heads/main aktualisiert.
marko@hp-lx:~/projects/git$ git log
commit d5c2136801551838a307dcc631689d803b71d9d5 (HEAD -> main)
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:35:40 2022 +0200

    amend! Three
    
    Three

commit 14bcd75a115b181ab1541904ba929c4cac034c35
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:29 2022 +0200

    Five

commit 513bc989cb28d51ec3aa06701baa24d3442c2eff
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:21 2022 +0200

    Four

commit c73bdb9a6ac122b778f5de40ad3a80e875ddcb1c
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:17 2022 +0200

    Three

commit 57769812c319524efaa96a8b9985a0c714061c09
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:12 2022 +0200

    Two

commit c30cc6c8750a50dfe0a15d529c400f45513637f7
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:26:25 2022 +0200

    One
marko@hp-lx:~/projects/git$ git rebase -i c73bdb9 --autosquash
Erfolgreich Rebase ausgeführt und refs/heads/main aktualisiert.
marko@hp-lx:~/projects/git$ git rebase -i c30cc --autosquash
automatischer Merge von hello.txt
KONFLIKT (Inhalt): Merge-Konflikt in hello.txt
error: Konnte d5c2136... (amend! Three) nicht anwenden
Hinweis: Resolve all conflicts manually, mark them as resolved with
Hinweis: "git add/rm <conflicted_files>", then run "git rebase --continue".
Hinweis: You can instead skip this commit: run "git rebase --skip".
Hinweis: To abort and get back to the state before "git rebase", run "git rebase --abort".
Konnte d5c2136... (amend! Three) nicht anwenden
marko@hp-lx:~/projects/git$ git log
commit c73bdb9a6ac122b778f5de40ad3a80e875ddcb1c (HEAD)
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:17 2022 +0200

    Three

commit 57769812c319524efaa96a8b9985a0c714061c09
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:27:12 2022 +0200

    Two

commit c30cc6c8750a50dfe0a15d529c400f45513637f7
Author: Marko <marko.beelmann@gmail.com>
Date:   Sun Jun 12 11:26:25 2022 +0200

    One

