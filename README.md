![Bloom Atten Header](docs/BloomAttenReadmeSS.png?raw=true "") 

# Bloom Attenuation
Tech demo to show a solution to improve traditional bloom. Bloom contribution is affected by depth buffer to simulate light attenuation. Implemented on Unity's Built-in Render Pipeline. \
\
     Full Explanation and breakdown: https://youtu.be/u5lX2zunj7g \
Project Source Available on Patreon: https://www.patreon.com/KH_Y

## To Start Tech Demo
***Windows 64-bit required** 
1. Clone or download zip with green "Code" button at the top right 
2. Run "BloomAttenutation.exe" (files must be unzipped)

## Controls
     WASD: to move
    Shift: run
    Space: jump

    Q: toggle Bloom Menu
    E: toggle Projectile Demo
    
    1: switch to default view
    2: switch to depth view
    3: switch to bloom contribution view
    
    p: toggle demo camera
    backspace: reload scene
    
## Bloom Parameters
**Blur iterations:** \
Number of iterations of down and upsampling with box sampling for blur.

**Threshold / Soft Threshold:** \
 *t* and *s*, respectively, in the bloom contribution function \
defined here: https://www.desmos.com/calculator/rauntuxt9o

**Intensity:** \
Intensity of bloom.

**Attenuation:** \
Normalized value for amount of bloom attenuation. Lerps between no attenuation (standard bloom) and full attenuation effect.

**Distance Scale:** \
Adjusts far plane of depth camera.

**Max Bloom Reduction:** \
Maximum amount of bloom that can be reduced by attenutation when objects are at/farther than depth camera's far plane.

