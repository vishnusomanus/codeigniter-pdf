# Codeigniter PDF
We can convert html to pdf in codeigniter using dompdf.



Download **/dompdf** folder and move it to **/system/helpers** folder.<br />
Download and upload **dompdf_helper.php** file to **/system/helpers**.<br />



## Use the given code in controller

    $this->load->helper(array('dompdf', 'file'));
    $html = $this->load->view('pdf/coupon', $data, true);
    pdf_create($html, 'filename');
