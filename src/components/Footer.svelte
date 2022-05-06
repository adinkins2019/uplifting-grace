<script>
   import SiteNav from './SiteNav.svelte'
</script>

<footer>
    <!-- Site Map-->
    <div>
        <SiteNav />
    </div>
    <!-- Copyright Information and Address -->
    <div class="copyright-info">
        <div>
            <address>
                124 Sumter Highway <br/>
                Bishopville, SC 29010
            </address>
            Telephone: <a href="tel:(803)123-4567">(803)123-4567</a>
        </div>
       <div id="copyright"> &copy; 2022. All Rights Reserved</div>
    </div>
    <!-- Social media links-->
    <div></div>
</footer>
<style>
    footer {
        display: flex;
        justify-content: space-around;
        align-items: flex-end;
        background: #71697A;
        font-weight: 500;
    }

    .copyright-info{
        display: flex;
        flex-direction: column;
        
    }
   #copyright {
       margin-top: 20px;
   }
</style>