I chose the materials jelly(ficus) an metal(plane) to simulate. The parameters were be edited in the config files ficus_config.json and plane_config.json. For jelly, I change the grid_v_damping_scale to 0.7 and 1.2(default is 0.9999). I also tried to set substep_dt to 1e-5(default is 1e-4), if I make it bigger of smaller, the running time of the code will increase considerably, so I just set one different substep_dt to run the code. The videos' links are below.  
defalut: https://youtube.com/shorts/K5uHghWVpr4?feature=share  
grid_v_damping_scale=0.7: https://youtube.com/shorts/Hq0V8PFoKqs?feature=share  
grid_v_damping_scale=1.2: https://youtube.com/shorts/8Wfd_K4I_yo?feature=share  
substep_dt=1e-5: https://youtube.com/shorts/lO_P9qfd5D4?feature=share  
I observed that grid_v_damping_scale mainly affect the amplitude that the branches swing. When grid_v_damping_scale inceased, the branches swang more obviously, while it almost not move when the value decreased. When I changed the substep_dt, the object is also motionless but I am not sure about the reason. The PSNR compared with the default video is:  
grid_v_damping_scale=0.7: 22.22dB  
grid_v_damping_scale=1.2: 20.30dB  
substep_dt=1e-5: 20.98dB

And for the metal simulation, I set substep_dt to 2e-4 adn n_grid to 100. The videos' links are below.  
default: https://youtube.com/shorts/y8IX0a19VFQ?feature=share  
substep_dt=2e-4: https://youtube.com/shorts/LKNxD0sKtvo?feature=share  
n_grid=100: https://youtube.com/shorts/5yznh-aypa8?feature=share
In this three videos, I didn't observe any obvious difference. The PSNR compared with the default video is:  
substep_dt=2e-4: 28.82dB  
n_grid=100: 27.72dB
