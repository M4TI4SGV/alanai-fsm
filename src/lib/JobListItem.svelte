<script>
    export let Client = ""
    export let JobTitle = ""
    export let Date = ""
    export let Time = ""
</script>

<li class="list-group-item list-group-item-action">
    <i class="fa fa-wrench"></i>
    {Client}
    <br>
    <i class="fa fa-user-circle"></i>
    {JobTitle}
    <div class="mrc-element">
        <i class="fa fa-calendar"></i>
        {Date} at {Time}
    </div>
</li>