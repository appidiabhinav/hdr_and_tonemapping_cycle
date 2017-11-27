# hdr_and_tonemapping_cycle

Implements a complete hdr and tonemapping cycle

 1: Computes the camera response curve according to "Recovering High
 Dynamic Range Radiance Maps from Photographs" by P. Debevec.
 
 You need a wide range of differently exposed pictures from the same scene
 to get good results.

 2: Recovers a hdr radiance map from the range of ldr pictures 

 3: Tonemaps the resulting hdr radiance map according to "Photographic
 Tone Reproduction for Digital Images" by Reinhard et al.
 
 Both the simple global and the more complex local tonemapping operator
 are applied to the hdr radiance map.

 Some code taken from Paul Debevec's implementation of his SIGGRAPH'97
 paper "Recovering High Dynamic Range Radiance Maps from Photographs"
