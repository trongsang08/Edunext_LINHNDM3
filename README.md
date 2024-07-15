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



2, const products = getProductsFromDatabase();

for (const product of products) {
  // Lấy mã sản phẩm
  const productId = product.id;

  // Lấy nút HTML tương ứng với mã sản phẩm
  const productButton = document.getElementById(`product-${productId}`);

  // Gắn sự kiện onclick cho nút HTML
  productButton.addEventListener('click', spanOnClick);
}
3,document.addEventListener('click', (event) => {
  if (event.target === spanOnClick) {
    // Lấy mã sản phẩm từ ID nút HTML
    const productId = parseInt(event.target.id.replace('product-', ''), 10);

    // Xử lý mã sản phẩm đã được nhấp
    handleProductClick(productId);
  }
});
4. function handleProductClick(productId) {
  // Hiển thị mô tả sản phẩm hoặc thực hiện hành động khác
  console.log(`Mã sản phẩm đã được nhấp: ${productId}`);
}
