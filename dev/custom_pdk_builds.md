

If you need custom libraries, you will have to resort to manual builds using Volare as shown below. You will need Git 2.35+ and Docker.

Note that this will take a while, from 20 minutes to an hour depending on your internet speed and compute power.

Start a venv shell using make start-build-env. You should see a prompt looking kind of like this:

(venv) [user@host openlane]$ 
First of all, install volare:

pip3 install --upgrade --no-cache-dir volare
Then, build the PDK as follows: The -l options are the libraries you want to include. For example, to also include sky130_fd_sc_hs, you can add -l sky130_fd_sc_hs to the default set of libraries using the following command:

volare build -j$(nproc) --pdk sky130 --clear-build-artifacts --sram -l sky130_fd_io -l sky130_fd_pr -l sky130_fd_sc_hvl -l sky130_fd_sc_hd -l sky130_fd_sc_hs
You can also add -l all to just include all of them:

volare build -j$(nproc) --pdk sky130 --clear-build-artifacts --sram -l all
Either way, go grab a smoothie. This will take a while.

After it is done, you can then enable the resulting PDK as such:

volare enable
Et voila, your custom-built PDK is ready.
