<template>
    <p style="text-align: center; font-size: large;">The 50 | 30 | 20 rule recommends putting 50% of your money toward needs, 30% toward wants, and 20%
        toward savings.</p>
    <div class="Chart">
        <img src="../assets/icons/Chart.png" alt="Chart showing the 50 | 30 | 20 rule." style="width: 50%; height: auto;">
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

    </div>
</template>

<style scoped>
.Chart{
    text-align: center;
    padding-bottom: 2rem;
    padding-top: 2rem;
    
}
.content {
    display: inline-block;
    text-align: left;
    margin-left: 5%;
    margin-right: 5%;
    width: 100%;
}
h2 {
    font-weight: bolder;
    text-decoration: underline;
}
p{
    padding: 1rem;
    width: 100%;
}
</style>