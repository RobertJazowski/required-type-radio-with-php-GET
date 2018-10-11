# required-type-radio-with-php-GET
single input returned to user on next page using php


<form action="submitpage1.php">
<p>
How would you rate your visit?<br>
<input id="RBHighSat"  required type="radio" name="ratevisit" value="Highly Satisfied">    <label for="RBHighSat"  >Highly Satisfied</label>
<input id="RBSat"      required type="radio" name="ratevisit" value="Satisfied">           <label for="RBSat"      >Satisfied</label>
<input id="RBNeithSorD"required type="radio" name="ratevisit" value="Neither Satisfied nor Dissatisfied"><label for="RBNeithSorD">Neither Satisfied nor Dissatisfied</label><br>
<input id="RBDiss"     required type="radio" name="ratevisit" value="Dissatisfied">        <label for="RBDiss"     >Dissatisfied</label>
<input id="RBHighDiss" required type="radio" name="ratevisit" value="Highly Dissatisfied"> <label for="RBHighDiss" >Highly Dissatisfied</label> 
</p>
<input type="submit" name="submit" value="Next" />
</form>
<?php
}else{
?>
<p>You entered: <?php echo $_GET['ratevisit']; ?></p>
<a href="submitpage2.php">
<input type="button" value="Next" />
</a>
<?php
}
?>
