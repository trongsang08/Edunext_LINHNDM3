# Edunext_LINHNDM3

function noneslides(slideindex, slidelength, slideindex, slidelength) {
  // None 2 slide trước slide hiện tại
  for (let i = slideindex - 2; i >= 0 && i < slidelength; i++) {
    document.getElementById(`slide-${i}`).style.display = "none";
  }

  // Block 2 slide sau slide hiện tại
  for (let i = slideindex + 2; i < slidelength; i++) {
    document.getElementById(`slide-${i}`).style.display = "block";
  }
}
