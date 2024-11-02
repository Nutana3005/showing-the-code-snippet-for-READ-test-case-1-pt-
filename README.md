# showing-the-code-snippet-for-READ-test-case-1-pt-
def test_create_product(self):
    product = ProductFactory()
    assert product is not None

def test_find_product_by_name(self):
    product = ProductFactory(name="Sample Product")
    found = Product.find_by_name("Sample Product")
    assert found == product
