<template>
    <div class="container">
        <h1>Financial Freedom 50 | 30 | 20 Rule </h1>

        <p>The 50 | 30 | 20 rule recommends putting 50% of your money toward needs, 30% toward wants, and 20% toward
            savings.</p>
    </div>
    <div>
        <img src="./icons/Chart.png" alt="Chart showing the 50 | 30 | 20 rule." style="width:650px;height:500px;">
    </div>
    <div class="Needs">

        <h2>Needs: 50%</h2>
        <p>
            These are expenses that must be met no matter what, such as:
            <li>Utility bills</li>
            <li>Rent or mortgage payments</li>
            <li>Health care</li>
            <li>Groceries</li>
            If you can honestly say “I can’t live without it,” you have identified a need. Minimum required payments on
            a
            credit card or a loan also belong in this category.
        </p>

    </div>
    <div class="Wants">
        <h2>Wants: 30%</h2>
        <p>
            Wants are things you enjoy that you spend money on by choice, not becuse you need it to live such as:
            <li>Subscriptions</li>
            <li>Supplies for hobbies</li>
            <li>Restaurant meals</li>
            <li>Vacations</li>
        </p>
    </div>
    <div class="Savings">
        <H2>Savings: 20%</H2>
        <p>The remaining 20% of your budget should go to your funding your future.
            You may put money in an emergency fund, contribute to a retirement account, or save toward a down payment on
            a home.
            Paying down debt beyond the minimum payment amount belongs in this category, too.</p>
    </div>

</template>

<style>
.Needs {
    border: solid;
    max-width: 44%;
    position: fixed;
    top: 200px;
    left: 0;

}

.Wants {
    border: solid;
    max-width: 44%;
    position: fixed;
    top: 500px;
    left: 0;

}

.Savings {
    border: solid;
    max-width: 44%;
    position: fixed;
    top: 700px;
    left: 0;

}


.container {
    text-align: center;
    text-wrap: pretty;
    position: fixed;
    top: 8px;
    left: 16px;
}

img {
    position: fixed;
    top: 20px;
    left: 300px;
}
</style>
