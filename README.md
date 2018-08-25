# bgp-path-hijacking-attack

Base code available here: https://bitbucket.org/jvimal/bgp

Code analized and commented for research purpose

---

## Quagga preparation

- download quagga-1.2.4 from [here](http://download.savannah.gnu.org/releases/quagga/) in your `$HOME` and extract it

- `cd ~/quagga-1.2.4`

- `chown mininet:mininet /var/run/quagga`

- edit `configure` file, add `${quagga_statedir_prefix}/var/run/quagga` before all options in `QUAGGA_STATE_DIR` for loop 

- `./configure --enable-user=mininet --enable-group=mininet`

- `make`
