# SMuRF defaults.yml files

One of the first things [pysmurf](https://github.com/slaclab/pysmurf)
does when it's initializing the SMuRF hardware is load the
defaults.yml file, which does a lot of the low level hardware
configuration, like configuring the SMuRF DACs, clocks, digitizers,
etc..

# defaults.yml variants

Here is an index of the defaults.yml files in this directory, along
with descriptions of he cases in which each should be used:

<table>  
<tr>  
      <th style="text-align:left; background-color: lightgray">defaults.yml</th>  
      <th style="text-align:left; background-color: lightgray">description</th>    
</tr>  
<tr>  
      <th colspan="2" style="background-color: lightgray">Single-bay</th>
</tr>
<tr>  
      <td><a href="defaults_c02_hb_none.yml">defaults_c02_hb_none.yml</a></td>  
      <td>
      For use with a HB AMC in bay 0, no AMC in bay 1.  For use with
      C02 AMCs (hence the "c02" in the name).
      </td>
</tr>
<tr>
      <td><a href="defaults_c03_hb_none.yml">defaults_c03_hb_none.yml</a></td>  
      <td>
      For use with a HB AMC in bay 0, no AMC in bay 1.  For use with
      C03 AMCs (hence the "c03" in the name).
      </td>      
</tr>
<tr>
      <td><a href="defaults_c02_lb_none.yml">defaults_c02_lb_none.yml</a></td>
      <td>
      For use with a LB AMC in bay 0, no AMC in bay 1.  For use with
      C02 AMCs (hence the "c02" in the name).
      </td>      
</tr>
<tr>
      <td><a href="defaults_c03_lb_none.yml">defaults_c03_lb_none.yml</a></td>
      <td>
      For use with a LB AMC in bay 0, no AMC in bay 1.  For use with
      C03 AMCs (hence the "c03" in the name).
      </td>            
</tr>
</tr>  
<tr>
      <th colspan="2" style="background-color: lightgray">Dual-bay</th>
<tr>
      <td><a href="defaults_c03_lb_hb.yml">defaults_c03_lb_hb.yml</a></td>  
      <td>
      For use with a LB AMC installed in bay 0, and a HB AMC installed
      in bay 1.  The carrier rev must be C02 or higher, and the AMC
      rev (for both the LB and HB AMCs) must be C03 or higher.
      </td>        
</tr>
<tr>
      <td><a href="defaults_c03_hb_lb.yml">defaults_c03_hb_lb.yml</a></td>  
      <td>
      For use with a HB AMC installed in bay 0, and a LB AMC installed
      in bay 1.  The carrier rev must be C02 or higher, and the AMC
      rev (for both the LB and HB AMCs) must be C03 or higher.      
      </td>
</tr>
<tr>
      <td><a href="2019_06_04_Dual_Band_AMC_Config_LBx2.yml">2019_06_04_Dual_Band_AMC_Config_LBx2.yml</a></td>  
      <td>
      For use with a LB AMCs installed in both bays.  The carrier rev
      must be C02 or higher, and the AMC rev (for both the LB and HB
      AMCs) must be C03 or higher.
      </td>
</tr>
<tr>
      <td><a href="defaults_c03_lb_lb.yml">defaults_c03_lb_lb.yml</a></td>  
      <td>
      For use with Rogue4 and LB AMCs installed in both bays.  The 
      carrier rev must be C02 or higher, and the AMC rev (for both 
      the LB AMCs) must be C03 or higher.
      </td>
</tr>
</tr>
</table>


