
### spinning up observer
```sh
function observerl
    set -l PATH /usr/local/lib/erlang/bin $PATH
    pkill -ilf observerl > /dev/null 2>&1
    sleep 1
    /usr/local/lib/erlang/bin/erl -name observerl -setcookie monster -s observer start -detached -start_epmd false
end
```
