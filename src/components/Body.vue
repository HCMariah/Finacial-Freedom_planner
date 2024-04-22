<script>
import Percentage from './Percentage.js'
</script>

<template>


    <div class="container">

        <p>The 50 | 30 | 20 rule recommends putting 50% of your money toward needs, 30% toward wants, and 20%
            toward savings.</p>
        <div>
            <img src="./icons/Chart.png" alt="Chart showing the 50 | 30 | 20 rule." width="80%" height="auto">
        </div>
        <div class="content">

            <div class="needs">
                <h2>Needs: 50%</h2>
                <p>
                    These are expenses that must be met no matter what, such as:
                    <li>Utility bills</li>
                    <li>Rent or mortgage payments</li>
                    <li>Health care</li>
                    <li>Groceries</li>
                    If you can honestly say “I can’t live without it,” you have identified a need. Minimum required
                    payments
                    on
                    a
                    credit card or a loan also belong in this category.
                </p>
            </div>
            <div class="wants">
                <h2>Wants: 30%</h2>
                <p>
                    Wants are things you enjoy that you spend money on by choice, not becuse you need it to live such
                    as:
                    <li>Subscriptions</li>
                    <li>Supplies for hobbies</li>
                    <li>Restaurant meals</li>
                    <li>Vacations</li>
                </p>
            </div>
            <div class="savings">
                <H2>Savings: 20%</H2>
                <p>The remaining 20% of your budget should go to your funding your future.
                    You may put money in an emergency fund, contribute to a retirement account, or save toward a down
                    payment on
                    a home.
                    Paying down debt beyond the minimum payment amount belongs in this category, too.</p>
            </div>
            <form>
                <label for="nbr">Monthly income : </label>
                <input type="number" id="nbr" placeholder="32000" maxlength="10">

                <input type="button" id="btn1" value="Submit">

                <p class="output" id="output1">Output</p>
            </form>


        </div>
    </div>

</template>



<style scoped>
.content {
    display: inline-block;
    text-align: left;

}

h2 {
    font-weight: bolder;
    text-decoration: underline;
}

form {
    margin-bottom: 20px;
}

input[type="number"] {
    padding: 5px;
    width: 200px;
}

button {
    padding: 5px 10px;
}
</style>