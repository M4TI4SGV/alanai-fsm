<script>
    import 'font-awesome/css/font-awesome.min.css';
    import JobListItem from '$lib/JobListItem.svelte';
</script>

<div class="row">
    <div class="col-12 col-lg-3 pr-0 pl-0 pl-lg-3">
        <ul class="list-group list-view overflow-auto" style="height: 90vh; max-width:500px">
            {#each Array(20) as _, i}
                <JobListItem Time="5:42 PM" JobTitle="Job #{i}" Client="Some Company"/>
            {/each}
        </ul>
    </div>
    <div class="col-lg-9 pl-0">
        <br>
        <div class="d-inline">
            <a class="btn btn-success" href="/add">
                <i class="fa fa-plus-circle"></i>
                Add New
            </a>
            <a class="btn btn-success" href="/dashboard/edit">
                <i class="fa fa-edit"></i>
                Edit
            </a>
            <a class="btn btn-primary" href="/dashboard/map">
                <i class="fa fa-map"></i>
                View Map
            </a>
        </div>
        <br><br>
        <slot />
    </div>
</div>