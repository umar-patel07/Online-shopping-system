// START WHEN THE DOCUMENT IS READY
if (document.readyState == "loading") {
    document.addEventListener('DOMContentLoaded', start);
} else {
    start();
}

// *****************START*******************
function start() {
    addEvents();

}

// *****************UPDATE & REMINDER*******************
function update() {
    addEvents();
    updateTotal();


}

// *****************ADD EVENTS*******************
function addEvents() {

    //REMOVE ITEMS FROM CART
    let cartRemove_btns = document.querySelectorAll('.cart-remove');
    console.log(cartRemove_btns);
    cartRemove_btns.forEach(btn => {
        btn.addEventListener("click", handle_removeCartItem);
    });

    // Change Item Quantity
    let cartQuantity_inputs = document.querySelectorAll('.cart-quantity');
    cartQuantity_inputs.forEach((input) => {
        input.addEventListener("change", handle_changeItemQuantity);
    });

    // Add Item To Cart
    let addCart_btns = document.querySelectorAll(".add-cart");
    addCart_btns.forEach(btn => {
        btn.addEventListener("click", handle_addCartItem);
    })

    // Buy Order
    const buy_btn = document.querySelector(".btn-buy");
    buy_btn.addEventListener("click", handle_buyOrder);
}


/*************HANDLE EVENTS FUNCTION***************** */
let itemsAdded = [];

function handle_addCartItem() {
    let product = this.parentElement;
    let title = product.querySelector(".card-title").innerHTML;
    let price = product.querySelector(".product-price").innerHTML;
    let imgsrc = product.querySelector(".product-image").src;
    console.log(title, price, imgsrc); // Correct the variable name to imgsrc

    let newToAdd = {
        title,
        price,
        imgsrc,
    };


    // Handle Item IS Already Exist
    if (itemsAdded.find((el) => el.title == newToAdd.title)) {
        alert("This Item Is Already Exist!");
        return;
    } else {
        itemsAdded.push(newToAdd);
    }

    // Add Product To Cart
    let cartBoxElement = CartBoxComponent(title, price, imgsrc);
    let newNode = document.createElement("div");
    newNode.innerHTML = cartBoxElement;
    const cartContent = cart.querySelector(".card");
    cartContent.appendChild(newNode);

    update();
}

function handle_removeCartItem() {
    this.parentElement.remove();
    itemsAdded = itemsAdded.filter(el => el.title != this.parentElement.querySelector(".text-center").innerHTML);
    update();
}

function handle_changeItemQuantity() {
    if (isNaN(this.value) || this.value < 1) {
        this.value = 1;
    }
    this.value = Math.floor(this.value); // To Keep It Integer
    update();
}

function handle_buyOrder() {
    if (itemsAdded.length <= 0) {
        alert("There Is No Order To Place Yet! \n Please Make An Order First.");
        return;
    }
    const cartContent = cart.querySelector(".card");
    cartContent.innerHTML = '';
    alert("Your Order Has Been Placed Successfully :)");
    itemsAdded = [];

    update();
}

/*************UPDATE FUNCTION***************** */
function updateTotal() {
    let cartBoxes = document.querySelectorAll('.cart-box');
    const totalElement = cart.querySelector('.total-price');
    let total = 0;
    cartBoxes.forEach(cartBox => {
        let priceElement = cartBox.querySelector('.cart-price');
        let price = parseFloat(priceElement.innerHTML.replace("₹", ""));
        let quantity = cartBox.querySelector('.cart-quantity').value;
        total += price * quantity;
    });

    // KEEP 2 digit After the Decimal Number
    total = total.toFixed(2);

    totalElement.innerHTML = "₹" + total;
}

// ======================HTML COMPONENTS==================
function CartBoxComponent(title, price, image) {
    return `
    <div class="col-md-3 py-3-md-0">
        <div class="card">
            <img src=${image} alt="Gaming Monitor" class="product-image"> <!-- Correct the variable name to image -->
            <div class="card-body">
                <h3 class="text-center card-title">${title}</h3>
                <p class="text-center">Lorem ipsum dolor sit amet.</p>
                <div class="star text-center">
                    <i class='bx bxs-star checked'></i>
                    <i class='bx bxs-star checked'></i>
                    <i class='bx bxs-star checked'></i>
                    <i class='bx bxs-star checked'></i>
                    <i class='bx bxs-star checked'></i>
                </div>
                <h2 class="product-price">${price}</h2>
                <a href="Cart.html"><li class="bx bxs-cart-alt add-cart"></li></a>
            </div>
        </div>
    </div>`;
}


// Function to update the timer display
function updateTimerDisplay(timeInSeconds) {
    const hours = Math.floor(timeInSeconds / 3600);
    const minutes = Math.floor((timeInSeconds % 3600) / 60);
    const seconds = timeInSeconds % 60;

    const formattedTime = `${String(hours).padStart(2, '0')}:${String(minutes).padStart(2, '0')}:${String(seconds).padStart(2, '0')}`;
    document.getElementById('timer').innerText = formattedTime;
}

// Function to start the countdown
function startCountdown() {
    let remainingTime = 5400; // 1 hour 30 minutes in seconds

    // Update the timer every second
    const timerInterval = setInterval(() => {
        remainingTime--;
        updateTimerDisplay(remainingTime);

        // End condition: when the timer reaches 0
        if (remainingTime <= 0) {
            clearInterval(timerInterval);
            document.getElementById('timer').innerText = "00:00:00"; // Display 00:00:00 at the end
        }
    }, 1000);
}

// Start the countdown when the page loads
startCountdown();