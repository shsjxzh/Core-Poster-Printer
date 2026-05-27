# Core Poster Printer Workflow

This is the Core poster printer workflow that has had the highest success rate for us. Adjust it as needed for your own poster.

## Steps

1. Log in to iLab through Weblogin:

   <https://weblogin.cs.rutgers.edu/guacamole-1.6.0/#/>

   <img src="core-poster-printer-assets/01-weblogin-home.png" alt="Weblogin page" width="500">

   <img src="core-poster-printer-assets/02-weblogin-ilab.png" alt="iLab connection page" width="500">

2. Download the poster you want to print, in PDF format, to the iLab server. Email, cloud storage, or similar file-transfer methods should work.

3. On the iLab virtual machine, open your poster with Atril Document Viewer. This is the only viewer that worked for us.

   <img src="core-poster-printer-assets/03-open-with-atril.png" alt="Opening the poster with Atril Document Viewer" width="500">

4. In Atril Document Viewer, press `Ctrl + P` and use the following settings.

   `General` -> `Printer` -> `artisan`

   <img src="core-poster-printer-assets/04-select-artisan-printer.png" alt="Selecting the artisan printer" width="500">

5. Switch to the `Page Setup` tab:

   <img src="core-poster-printer-assets/07-page-setup-summary-2.png" alt="Example Page Setup screen" width="650">

   - `Scale`: Calculate the scale based on your poster dimensions.

      > Make **absolutely sure** the shorter side of the poster is scaled to `36 in`. This printer cannot print posters wider than that.

      For example, if the poster PDF is `48 in x 24 in` and you want a real poster size of `72 in x 36 in`, use `150%` as the scale.

      If you do not know the original size of the PDF, click `File` -> `Properties` in the Atril menu bar.

   - `Paper Size`: Select `Custom Size`, then enter the actual poster size **after scaling**. In the example above, the scaled size is `72 in x 36 in`.

      > Enter `36` for `Width` and `72` for `Height`. Even if your poster is horizontal, the printer's maximum width is `36`, so the poster will be printed vertically. If `Width` is larger than `36`, the printer may have issues.

      For the `Margins` setting, click `Margins from Printer` to use the margins from the printer settings.

      <img src="core-poster-printer-assets/06-custom-paper-size-2.png" alt="Setting a custom paper size" width="520">

   - `Orientation`: After the page size is set, the paper orientation will automatically become landscape or portrait.

6. Switch to the `Page Handling` tab and use the settings shown below.

   <img src="core-poster-printer-assets/06-page-handling.png" alt="Page Handling settings" width="520">

7. Click `Preview`, which is next to the `Print` button. Confirm that the poster orientation and scale are correct and that there is not a large amount of white space.

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

8. Click `Print`, then go to the Core 3rd-floor print room and wait for the poster to print.

   If a size warning appears, press `Print Anyway` on the printer. It is the second option from the left. If the print job stops or errors for another reason, restart the printer. If the issue continues, call the phone number posted on the wall.

   Core 3rd-floor printer:

   <img src="core-poster-printer-assets/10-core-third-floor-printer.jpeg" alt="Core 3rd-floor printer" width="500">

## Finished Poster

<img src="core-poster-printer-assets/11-finished-poster.jpeg" alt="Finished poster" width="650">

## Notes

- You can ignore the printer warnings shown below. If the printer is actually out of ink, contact staff using the phone number posted on the wall.

<img src="core-poster-printer-assets/12-printer-warnings.jpeg" alt="Printer warning examples" width="500">

- If the phone number does not work either, go directly to the LCSR Operator in CoRE 235. If no one is in CoRE 235, ask staff in the nearby LCSR offices. They are also familiar with the printer.

- After submitting the print job, it is normal for it to stay pending briefly. On the campus network, you can check the job status at [https://printserver.cs.rutgers.edu/jobs/](https://printserver.cs.rutgers.edu/jobs/). If nothing happens for more than 15 minutes, check the printer status in the iLab terminal:

   ```bash
   lpstat -p artisan
   ```

   If the status looks like this, contact school staff:

   ```bash
   printer artisan disabled since <time> -
	cfFilterChain: pdftopdf (PID 2520749) exited with no errors.
   ```

   This status means the printer is working:

   ```bash
   printer artisan is idle.  enabled since <time>
   ```
