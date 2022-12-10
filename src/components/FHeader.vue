<template>
    <div>
        <div>
            <b-card title="Card Title" no-body>
                <b-card-header header-tag="nav">
                    <b-nav align="center" card-header pills>
                        <h1>{{header_name}}</h1>
                        <b-icon icon="emoji-smile-fill" font-scale="3"></b-icon>
                    </b-nav>
                </b-card-header>
            </b-card>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'F-Header',
        data(){
            return({
                msg: 'F-Header'
            })
        },
        props: ['header_name']
    }
</script>