**Overview:** This guide provides step-by-step instructions on how to use prepare-nf in EPI2ME, Oxford Nanopore Technologies’ cloud-based data analysis platform. It can be used to create a sample sheet to be used as input file in the ARTIC bioinformatics amplicon-nf pipeline on a Desktop or Laptop computer without having to use a command-line interface.

**Requirements:**

* EPI2ME installed. Further instructions can be found at XXX.
* Internet access to download the pipeline, and for the first time running it. After that, you should be able to run it offline.
* Details about sample names, barcode assignment, and any other metadata required for analysis. These should be collated in a CSV or XLS file using the template in XXX, and containing the following required columns:
	* Sample name (e.g., sample1)
	* Barcode (e.g. barcode01)
	* any other columns with additional information

---

## Using the ARTIC prepare-nf analysis pipeline in EPI2ME

## ---

### **Import the workflow**

Open EPI2ME. From the left-hand side panel, select "Launch". 

![](/images/prepare-nf/Screenshot_preparenf_launch.png)

Then select “Import workflow” and "Import from Github".

![](/images/prepare-nf/Screenshot_preparenf_import.png)

A pop-up window will appear where you can enter the GitHub URL. Enter the URL and click “Download” ([https://github.com/artic-network/prepare-nf](https://github.com/artic-network/prepare-nf "Prepare-nf download link")):

![](/images/prepare-nf/Screenshot_preparenf_link.png)

Once it has downloaded, it will be ready in the Available Workflows tab. Select it and you will be taken to a landing page for this workflow.

### **Running the workflow**

From the workflow landing page, click “Launch”.

![](/images/prepare-nf/Screenshot_preparenf_initiate.png)

Select the appropriate technology form the “Sequencing platform” drop down menu, along with the path to the fastq files directory in “Run Directory”. 

![](/images/prepare-nf/Screenshot_preparenf_platform_directory.png)

Next, browse for and select the CSV or XLS file containing your metadata in the “Metadata” section. 

Enter the name of the amplicon scheme using the nomenclature in Pimalscheme labs ([https://labs.primalscheme.com](https://labs.primalscheme.com)), e.g., artic-inrb-mpox/2500/v1.0.0. Make sure that the primer scheme matches the one you used for your sequencing. 

(TO EDIT: if scheme not available...)

![](/images/prepare-nf/Screenshot_preparenf_metadata_amplicon.png)

Finally click “Launch workflow” and “Launch” in the pop up window to initiate the workflow. You will be redirected to the “Progress” panel with bars indicating the run progress. The runtime will depend on the size of your files and the speed of your computer, but it usually takes XXX minutes. The bar will change to green and ‘Complete’ when it has finished.
 
(TO ADD: screenshot)

When it has finished you will have a file called sample_config.csv. You can feed this into amplicon-nf to proceed with your analysis.

(TO ADD: screenshot – example of csv file)