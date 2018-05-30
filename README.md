# centos-recipes
**Receitas do *CentOS***

- Buscar pacotes instalados: rpm -qa | grep -i 'php*'
- Buscar pacotes disponívels: yum search php-
- Gravar output em arquivo: php -i > "g.txt"
- lsof -i :8090
- pkill -f processosparafechar
- kill -9 pid
- killall -9 nome
- pgrep node
- ps aux | grep firefox
- Utilização de CPU: mpstat -P ALL OU mpstat | grep -A 5 "%idle" | tail -n 1 | awk -F " " '{print 100 -  $ 12}'a
- Utilização de CPU: sar
- Filtrar uso de CPU: ps -eo pcpu,pid,user,args | sort -k 1 -r | head -10 OU ps -eo pcpu,pid,user,args | sort -r -k1 | less
- Utilização de CPU: iostat
- Utilização de memória: free -t -m
- Utilização de memória: cat /proc/meminfo
- Utilização de memória: top
- Utilização de memória: vmstat -s
- Monitorar utilização: watch -n 5 free -m
