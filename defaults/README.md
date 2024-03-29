# SMuRF defaults.yml files

The pysmurf server usually detects one of the following configuration files,
otherwise it must be specified manually in start\_server.sh.  it sets various
parameters at the firmware level, like configuring the SMuRF DACs, clocks, and
digitizers. 

The file format is defaults\_version\_bay0type\_bay1type.yml.

- version: c02, c03. The version of the AMC mezzanine cards in both bay 0 and bay 1.
- bay0type: hb, lb. The type of AMC in bay 0, which is on the right hand side facing the carrier bays.
- bay1type: hb, lb. The type of AMC in bay 1, on the left.

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
<tr>
      <td><a href="defaults_c03_tkid_none_480MHz.yml">defaults_c03_tkid_none_480MHz.yml</a></td>  
      <td>
      For use with Rogue4 and a TKID AMC installed in bay 0.  Assumes
      the carrier rev is <b>C01</b> (the only difference between this and
      the defaults.ymls for later rev carriers is that we bypass the
      JESD sysref min/max check) and the AMC base board rev is C03.
      Programs the ADC/DAC LO to 480 MHz.
      </td>
</tr>
<tr>
      <td><a href="defaults_c03_tkid_none_595pt2MHz.yml">defaults_c03_tkid_none_595pt2MHz.yml</a></td>  
      <td>
      For use with Rogue4 and a TKID AMC installed in bay 0.  Assumes
      the carrier rev is <b>C01</b> (the only difference between this and
      the defaults.ymls for later rev carriers is that we bypass the
      JESD sysref min/max check) and the AMC base board rev is C03.
      Programs the ADC/DAC LO to 595.2 MHz.
      </td>
</tr>
<tr>
      <td><a href="defaults_c03_tkid_none.yml">defaults_c03_tkid_none.yml</a></td>  
      <td>
      For use with Rogue4 and a TKID AMC installed in bay 0.  Assumes
      the carrier rev is <b>C01</b> (the only difference between this
      and the defaults.ymls for later rev carriers is that we bypass
      the JESD sysref min/max check) and the AMC base board rev is
      C03.  This soft link determines which defaults yml is used if
      the SMuRF server is booted with hardware detection enabled
      (where currently the only difference between defaults is the LO
      frequency).
      </td>
</tr>
<tr>
      <td><a href="defaults_rfsoc_zcu208.yml">defaults_rfsoc_zcu208.yml</a></td>  
      <td>
      For use with Rogue4 and the RFSoC SMuRF port to the Xilinx ZCU208 evaluation board.
      </td>
</tr>
</tr>
</table>


