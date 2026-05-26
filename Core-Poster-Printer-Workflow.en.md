# Core Poster Printer Workflow

This is the Core poster printer workflow that has had the highest success rate for us. Adjust it as needed for your own poster.

## Steps

1. Log in to iLab through Weblogin:

   <https://weblogin.cs.rutgers.edu/guacamole-1.5.5/#/>

   <img src="core-poster-printer-assets/01-weblogin-home.png" alt="Weblogin page" width="500">

   <img src="core-poster-printer-assets/02-weblogin-ilab.png" alt="iLab connection page" width="500">

2. Download the poster you want to print, in PDF format, to the iLab server. Email, cloud storage, or similar file-transfer methods should work.

3. On the iLab virtual machine, open your poster with Atril Document Viewer. This is the only viewer that worked for us.

   <img src="core-poster-printer-assets/03-open-with-atril.png" alt="Opening the poster with Atril Document Viewer" width="500">

4. **Calculate** the scale based on your poster dimensions. **Make sure the shorter side of the poster is scaled to `36 in`**.

   For example, if the original poster size is `53.3 in x 30 in`, use `120%` as the scale. The final poster size will be `64 in x 36 in`.

5. In Atril Document Viewer, press `Ctrl + P` and use the following settings.

   `General` -> `Printer` -> `artisan`

   <img src="core-poster-printer-assets/04-select-artisan-printer.png" alt="Selecting the artisan printer" width="500">

   `Page Setup`:

   - `Scale`: Enter the **percentage calculated in step 4**. For the `53.3 in x 30 in` example above, use `120%`.
   - `Orientation`: Select `Landscape`. This assumes the poster text is arranged horizontally.

   ![Setting the orientation to Landscape](core-poster-printer-assets/05-orientation-landscape.png)

   - `Paper Size`: Select `Custom Size`, then enter the actual poster size **after scaling**. In the example above, the scaled size is `64 in x 36 in`, so enter `64` for `Width` and `36` for `Height`. You do not need to change the margins.

   <br>

   <img src="core-poster-printer-assets/06-custom-paper-size.png" alt="Setting a custom paper size" width="520">

   Example `Page Setup` screen:

   <img src="core-poster-printer-assets/07-page-setup-summary.png" alt="Example Page Setup screen" width="650">

6. Click `Preview`, which is next to the `Print` button. Confirm that the poster orientation and scale are correct and that there is not a large amount of white space.

   <table>
     <tr>
       <th>Correct ✔</th>
       <th>Incorrect ✘</th>
     </tr>
     <tr>
       <td valign="top">
         <img src="core-poster-printer-assets/09-preview-correct.png" alt="Correct preview example" width="360">
       </td>
       <td valign="top">
         <img src="core-poster-printer-assets/08-preview-wrong.png" alt="Incorrect preview example" width="360">
       </td>
     </tr>
   </table>

7. Click `Print`, then go to the Core 3rd-floor print room and wait for the poster to print.

   If a size warning appears, press `Print Anyway` on the printer. It is the second option from the left. If the print job stops or errors for another reason, restart the printer. If the issue continues, call the phone number posted on the wall.

   Core 3rd-floor printer:

   <img src="core-poster-printer-assets/10-core-third-floor-printer.jpeg" alt="Core 3rd-floor printer" width="500">

## Finished Poster

<img src="core-poster-printer-assets/11-finished-poster.jpeg" alt="Finished poster" width="650">

## Notes

You can ignore the printer warnings shown below. If the printer is actually out of ink, contact staff using the phone number posted on the wall.

<img src="core-poster-printer-assets/12-printer-warnings.jpeg" alt="Printer warning examples" width="500">
